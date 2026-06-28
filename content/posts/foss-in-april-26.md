+++
date = "2026-04-30 11:11:11 +0530"
title = "FOSS Activities in April 2026"
slug = "foss-in-april-26"
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

- Leading the DebConf Bursary team along with PEB.
  - This took most of my Debian time this month and I think it'll be the same next month, too.
- Assisted a few folks in getting their patches submitted via Salsa.
- Mentoring for newcomers.
- Moderation of -project mailing list.

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

I joined [Canonical to work on Ubuntu full-time](https://utkarsh2102.org/posts/hello-canonical/) back in February 2021.

Whilst I can't give a full, detailed list of things I did, here's a quick TL;DR of what I did:

- Successfully released [26.04 LTS](https://discourse.ubuntu.com/t/ubuntu-26-04-resolute-raccoon-lts-released/80833)!
  - It was a smooth release - thank you to everyone who helped get us here. \o/
- Started working on 26.10 archive opening.
  - It's codenamed Stonking Stingray!
- Assisted a bunch of folks with my Archive Admin and Release team hats to:
  - Review and grant FFes.
  - Accepted bug fixes during the freezes.
  - Coordinating weekly syncs.
  - Promoting/demoting binaries to/from main.
  - Taking care of package removals and so on.
- Was pretty occupied with the new release process architecture and design.
- Preparing for the Madrid sprints.

---

## Debian (E)LTS
{{< figure src="/images/debian-lts-small.png" >}}

This month I have worked 9 hours
on [Debian Long Term Support (LTS)](https://www.freexian.com/lts/debian/)
and on its sister [Extended LTS](https://www.freexian.com/lts/extended/)
project and did the following things:

### Work in Progress

- **php-phpseclib**: Affected by CVE-2023-52892 and CVE-2026-32935, at the moment.
  - **[LTS]**: Prepared 2.0.30-2+deb11u3 with the two CVEs mentioned above.
  - There might be more CVEs coming. I'll carry over the work to next month.

- **knot-resolver**: Affected by CVE-2023-26249, CVE-2023-46317, and CVE-2022-40188, leading to Denial of Service.
  - **[LTS]**: Still in back and forth discussion with maintainers on the best way to proceed for the bullseye upload. Git repository for bullseye: https://salsa.debian.org/lts-team/packages/knot-resolver/-/tree/debian/bullseye.
  - Carry-over'd from last month.

- **node-lodash**: Affected by [CVE-2025-13465](https://security-tracker.debian.org/tracker/CVE-2025-13465), prototype pollution in the `baseUnset` function.
  - **[stable]**: Xavier from the JS team ACK'd the patch. The trixie and bookworm uploads will follow.
  - **[LTS]**: The bullseye test and upload will follow once the stable uploads are in and ACK'd by the SRMs.
  - Carry-over'd from last month.

### Other Activities

- **[E/LTS] Front Desk duties**: Performed a large batch of CVE triage, marking numerous packages for bullseye, buster, and stretch as either `postponed`, `end-of-life`, `not-affected`, or added them to the Xla-needed.txt files.
  - Also replied to certain mails and IRC texts around FD related tasks.

- **[ELTS]** Still looking at ruby-rack and its monstrosity. :)

- **[E/LTS]** Monitored discussions on mailing lists, IRC, and all the documentation updates.

---

Until next time.  
`:wq` for today.
