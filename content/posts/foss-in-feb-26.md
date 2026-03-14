+++
date = "2026-02-28 11:11:11 +0530"
title = "FOSS Activites in February 2026"
slug = "foss-in-feb-26"
images = [
    "/images/debian-logo-small.png",
    "/images/ubuntu-logo-small.png",
    "/images/debian-lts-small.png",
]
tags = [
    "debian",
    "ubuntu",
    "monthly",
]
categories = [
    "debian",
    "ubuntu",
    "open-source",
]
+++

Here's my monthly but brief update about the activities I've done in the FOSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

Whilst I didn't get a chance to do much, here are still a few things that I worked on:

- Uploaded node-lodash/4.17.21+dfsg+~cs8.31.198.20210220-10 to fix CVE-2025-13465 in unstable. Pinged Xavier and Praveen to see how they feel about the backport for the stable releases.
- Assited a few folks in getting their patches submitted via Salsa.
  - Reviewing pyenv MR for Ujjwal.
  - Reviewing and assisting Anshul with his Golang stuff.
- Mentoring for newcomers.
- Started to be a bit involved with DC 26 bits.
- Moderation of -project mailing list.

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

I joined [Canonical to work on Ubuntu full-time](https://utkarsh2102.org/posts/hello-canonical/) back in February 2021.

Whilst I can't give a full, detailed list of things I did, here's a quick TL;DR of what I did:

- Successfully released [Resolute Snapshot 4](https://discourse.ubuntu.com/t/resolute-snapshot-4-released/77687)!
  - This one was also done without the ISO tracker and cdimage access.
  - We also worked very hard to build and promote all the image in due time.
  - This was one done with the Test Observer. The first one.
- Worked further on the whole artifact signing story for cdimage.
- Assisted a bunch of folks with my Archive Admin and Release team hats to:
  - Review and grant FFes.
  - Coordinating weekly syncs.
  - Promoting binaries to main.
  - Taking care of package removals and so on.
- Was pretty occupied with the new release processs architecture.

---

## Debian (E)LTS
{{< figure src="/images/debian-lts-small.png" >}}

This month I have worked 42 hours
on [Debian Long Term Support (LTS)](https://www.freexian.com/lts/debian/)
and on its sister [Extended LTS](https://www.freexian.com/lts/extended/)
project and did the following things:

### Released Security Updates

- **xrdp**: Unauthenticated stack-based buffer overflow in the RDP server.
  - **[LTS]**: Fixed [CVE-2025-68670](https://security-tracker.debian.org/tracker/CVE-2025-68670) via [**0.9.21.1-1~deb11u3**](https://tracker.debian.org/news/1712208/accepted-xrdp-09211-1deb11u3-source-into-oldoldstable-security/) for bullseye. This has been released as [**DLA 4464-1**](https://www.debian.org/lts/security/2026/DLA-4464-1).
  - **[ELTS]**: Fixed [CVE-2025-68670](https://security-tracker.debian.org/tracker/CVE-2025-68670) for buster via **0.9.9-1+deb10u5**. This has been released as [**ELA 1636-1**](https://www.freexian.com/lts/extended/updates/ela-1636-1-xrdp/).

- **phpunit**: Unsafe deserialization of code coverage data in PHPT test execution.
  - **[LTS]**: Fixed [CVE-2026-24765](https://security-tracker.debian.org/tracker/CVE-2026-24765) via [**9.5.2-1+deb11u1**](https://tracker.debian.org/news/1713511/accepted-phpunit-952-1deb11u1-source-into-oldoldstable-security/) for bullseye. This has been released as [**DLA 4470-1**](https://www.debian.org/lts/security/2026/DLA-4470-1).
  - **[ELTS]**: Fixed [CVE-2026-24765](https://security-tracker.debian.org/tracker/CVE-2026-24765) for buster via **7.5.6-1+deb10u1**. This has been released as [**ELA 1638-1**](https://www.freexian.com/lts/extended/updates/ela-1638-1-phpunit/).


### Work in Progress

- **knot-resolver**: Affected by CVE-2023-26249, CVE-2023-46317, and CVE-2022-40188, leading to Denial of Service.
  - **[LTS]**: Some back and forth discussion with maintainers on the best way to proceed for the bullseye upload.
    - Git repository for bullseye: https://salsa.debian.org/lts-team/packages/knot-resolver/-/tree/debian/bullseye.

- **ruby-rack**: There were multiple vulnerabilities reported in Rack, leading to DoS (memory exhaustion) and proxy bypass.
  - **[ELTS]**: I've partially reviewed patches by Bastien but whilst doing so, new ones came up for all the releases.
  - **[sid]**: Uploaded ruby-rack/3.2.5-1 to unstable to fix the new CVEs, CVE-2026-25500 and CVE-2026-22860.
  - **[stable]**: Prepared the upload for stable releases, as requested by the Security Team. Will upload them in March.
  - **[bullseye]**: Backport for CVE-2026-22860 hasn't been as trivial as it appears to be. There are test failures, which aren't really ignore-able:
    > The tests requests `/cgi/../test`, which `File.expand_path` resolves to `<root>/test` - firmly inside `@root`. With the old code, it hit the return `unless path_info.include? ".."` guard and fell through to 403. But it would also have returned early via `start_with?(@root)` being true…
  - ...anyway, this needs more investigation - I'll continue to do so in March as P1.

- **node-lodash**: Affected by CVE-2025-13465, lrototype pollution in baseUnset function.
  - **[stable]**: The patch for trixie and bookworm are ready and have been awaiting the maintainer review.
  - **[LTS]**: The bullseye upload will follow once the stable uploads are in and ACK'd by the SRMs.

- **vlc**: Affected by CVE-2025-51602, an out-of-bounds read and denial of service via a crafted 0x01 response from an MMS server.
  - **[LTS]**: 3.0.23 backport is ready but not tested. I'll get this over the line in March.
  - **[ELTS]**: 3.0.23 backport is ready but not very clean. Would like to complete LTS and get back to this.


### Other Activities

- **[LTS] Front Desk duties**: Performed a large batch of CVE triage, marking numerous packages for bullseye, buster, and stretch as either `postponed`, `end-of-life`, `not-affected`, or added them to the Xla-needed.txt files.
  - Also replied to certain mails and IRC texts around FD related tasks.

- **[ELTS]** Continued to help Bastien and Markus with the tomcat9 regression for buster.

- **[ELTS]** Partially reviewed ruby-rack CVEs to help Bastien. This took more time than expected with some more develpments hapening at the end of the month - new CVEs that aren't as easy to backport as I expected them to be. Will continue with these in March.

- **[LTS]** Coordinated the libvirt sitaution with Ben Hutchings. The upload has already been prepped, will upload in March.

- **[LTS]** Attended the monthly LTS meeting on Jitsi. [Summary here](https://lists.debian.org/debian-lts/2026/02/msg00026.html).

- **[E/LTS]** Monitored discussions on mailing lists, IRC, and all the documentation updates.

---

Until next time.  
`:wq` for today.
