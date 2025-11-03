+++
date = "2025-10-30 11:11:11 +0530"
title = "FOSS Activites in October 2025"
slug = "foss-in-oct-25"
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

Here's my monthly but brief update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

Whilst I didn't get a chance to do much, here's still a few things that I worked on:

- Uploaded ruby-rack, 3.1.18-1, to fix a bunch of CVEs.
- Asssited a few folks in getting their patches submitted via Salsa.
- Mentoring for newcomers.
- Moderation of -project mailing list.

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

I joined [Canonical to work on Ubuntu full-time](https://utkarsh2102.org/posts/hello-canonical/) back in February 2021.

Whilst I can't give a full, detailed list of things I did, here's a quick TL;DR of what I did:

- Successfully released [Ubuntu 25.10 - Questing Quokka](https://discourse.ubuntu.com/t/ubuntu-25-10-questing-quokka-released/69067)!
  - This one was particularly interesting as I pressed the "release" button at 8:30 AM from my room. :)
  - The earliest we've ever released so far!
- Started work on archive opening and [Resolute Raccoon is now open for development](https://lists.ubuntu.com/archives/ubuntu-devel/2025-October/043470.html)!
- I also attended the Ubuntu Summit held in London this time.
  - I even gave a talk about "[Ubuntu’s Monthly Snapshots: Why We Did This to Ourselves](https://discourse.ubuntu.com/t/ubuntu-s-monthly-snapshots-why-we-did-this-to-ourselves/67261/1)".
- From there, I flew to Gothenburg, Sweden to attend the product roadmap & engineering sprints.

---

## Debian (E)LTS
{{< figure src="/images/debian-lts-small.png" >}}

This month I have worked
16 hours on [Debian Long Term Support (LTS)](https://www.freexian.com/lts/debian/) and
05 hours on its sister [Extended LTS](https://www.freexian.com/lts/extended/) project and
did the following things:


- **ruby-rack**: There were multiple vulnerabilities reported leading to DoS (memory exhaustion) and proxy bypass.
  - **[unstable/forky]**: Uploaded a [fix to **unstable** via **3.1.18-1**](https://tracker.debian.org/news/1684537/accepted-ruby-rack-3118-1-source-into-unstable/) to fix 5 CVEs.
  - **[trixie/bookworm]**: Uploaded a fix for all 5 CVEs in **trixie** via **3.1.18-1~deb13u1** and 7 CVEs in **bookworm** via **2.2.20-0+deb12u1**.
  - **[LTS]**: Uploaded a fix for all 7 CVEs in **bullseye** via **2.1.4-3+deb11u4**. And released [DLA 4357-1](https://lists.debian.org/debian-lts-announce/2025/11/msg00000.html).
  - **[ELTS]**: Backported fixes for CVE-2025-46727 & CVE-2025-32441 to buster and stretch but the other backports are being a bit tricky due to really old versions. But I'll spend some more time there before coming to a conclusion.

- **wordpress**: There were multiple vulnerabilities reported leading to Sent Data & Cross-site Scripting.
  - **[bookworm]**: Uploaded a fix for all 4 CVEs in **bookwrom** via **6.1.9+dfsg1-0+deb12u1**.
  - **[LTS]**: Uploaded a fix for all 4 CVEs in **bullseye** via **5.7.14+dfsg1-0+deb11u1**. And released [DLA 4358-1](https://lists.debian.org/debian-lts-announce/2025/11/msg00001.html).

- **[LTS]** Attended the monthly LTS meeting on Jitsi. [Summary here](https://lists.debian.org/debian-lts/2025/10/msg00026.html).

- **[E/LTS]** Monitored discussions on mailing lists, IRC, and all the documentation updates.

---

Until next time.  
`:wq` for today.
