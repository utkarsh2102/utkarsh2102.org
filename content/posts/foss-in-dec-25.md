+++
date = "2025-12-30 11:11:11 +0530"
title = "FOSS Activites in December 2025"
slug = "foss-in-dec-25"
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

- Prepared security update for wordpress for trixie and bookworm.
- A few discussions with the new DFSG team, et al.
- Assited a few folks in getting their patches submitted via Salsa.
- Mentoring for newcomers.
- Moderation of -project mailing list.

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

I joined [Canonical to work on Ubuntu full-time](https://utkarsh2102.org/posts/hello-canonical/) back in February 2021.

Whilst I can't give a full, detailed list of things I did, here's a quick TL;DR of what I did:

- Successfully released [Resolute Snapshot 2](https://discourse.ubuntu.com/t/resolute-snapshot-2-released/73478)!
  - This one was also done without the ISO tracker and cdimage access.
  - I think this one went rather smooth. Let's see what we're able to do for snapshot 3.
- Worked on removing GPG keys from the cdimage instance. That took a while, whew!
- Assisted a bunch of folks with my Archive Admin and Release team hats to:
  - review NEW packages for Ubuntu Studio.
  - remove old binaries that are stalling transition and/or migration.
  - LTS requalification of Ubuntu flavours.
  - bootstrapping dotnet-10 packages for Stable Release Updates.
- With that, we've entered the EOY break. :)

---

## Debian (E)LTS
{{< figure src="/images/debian-lts-small.png" >}}

This month I have worked FIXME:65 hours
on [Debian Long Term Support (LTS)](https://www.freexian.com/lts/debian/)
and on its sister [Extended LTS](https://www.freexian.com/lts/extended/)
project and did the following things:


- **wordpress**: There were multiple vulnerabilities reported in Wordpress, leading to Sent Data & Cross-site Scripting.
  - **[bookworm]**: Roberto rightly pointed out that the upload to bookworm hadn't gone through last month, so I re-uploaded **wordpress/6.1.9+dfsg1-0+deb12u1** to **bookworm-security**.
  - This is now released as [DSA 6075-1](https://lists.debian.org/debian-security-announce/2025/msg00241.html).

- **ruby-rack**: There were multiple vulnerabilities reported in Rack, leading to DoS (memory exhaustion) and proxy bypass.
  - **[ELTS]**: Last month I had backported fixes for CVE-2025-46727 & CVE-2025-32441 to buster and stretch but the other backports were being a bit tricky due to really old versions.
  - I spent a bit more time but there's a lot to demystify. Gonna take a bit of break from this one and come back to this after doing other updates. Might even consider sending a RFH to the list.

- **libwebsockets**: Multiple issues were reported in LWS causing denial of service and stack-based buffer overflow.
  - **[LTS]**: For **bullseye**, these were [fixed via **4.0.20-2+deb11u1**](https://tracker.debian.org/news/1689800/accepted-libwebsockets-4020-2deb11u1-source-into-oldoldstable-security/). And released as [DLA 4373-1](https://lists.debian.org/debian-lts-announce/2025/11/msg00016.html).

- **mako**: It was found that Mako, a Python template library, was vulnerable to a denial of service attack via crafted regular expressions.
  - **[LTS]**: For **bullseye**, these were [fixed via **1.1.3+ds1-2+deb11u1**](https://tracker.debian.org/news/1694871/accepted-mako-113ds1-2deb11u1-source-into-oldoldstable-security/). And released as [DLA 4393-1](https://lists.debian.org/debian-lts-announce/2025/12/msg00004.html).
  - Backporting tests was an interesting exercise as I had to make them compatible with the bullseye version. :)

- **ceph**: Affected by CVE-2024-47866, using the argument `x-amz-copy-source` to put an object and specifying an empty string as its content leads to the RGW daemon crashing, resulting in a DoS attack.
  - **[LTS]**: Whilst the patch is straightforward, backports are a bit tricky. I've prepared the update but would like to reach out to zigo, the maintainer, to make sure nothing regresses.
  - **[ELTS]**: Same as LTS, I'd like to get a quick review and upload to LTS first before I start staging uploads for ELTS.

- **[LTS]** Attended the monthly LTS meeting on IRC. [Summary here](https://lists.debian.org/debian-lts/2025/11/msg00023.html).
  - It was also followed by a 50-minute post-meeting technical discussion/question session.

- **[E/LTS]** Monitored discussions on mailing lists, IRC, and all the documentation updates. Thanks, Sylvain, for a great documentation summary.

---

Until next time.  
`:wq` for today.
