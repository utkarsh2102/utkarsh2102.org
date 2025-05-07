+++
date = "2025-04-30 11:11:11 +0530"
title = "FOSS Activites in April 2025"
slug = "foss-in-april-25"
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

Here's my 67th monthly but brief update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 76th month of actively contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March 2019 and a [DD](https://wiki.debian.org/DebianDeveloper) on Christmas '19! \o/

There's a bunch of things I do, both, technical and non-technical. Here's what I did:

- Updating Matomo to v5.3.1.
- Lots of bursary stuff for DC25. We rolled out the results for the first batch.
- Helping Andreas Tille with and around FTP team bits.
- Mentoring for newcomers.
- Moderation of -project mailing list.

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

This was my 51st month of actively contributing to [Ubuntu](https://ubuntu.com/about).
I joined [Canonical to work on Ubuntu full-time](https://utkarsh2102.org/posts/hello-canonical/) back in February 2021.

Whilst I can't give a full, detailed list of things I did (there's so much and some of it might not be public...yet!), here's a quick TL;DR of what I did:

- [Released 25.04 Plucky Puffin](https://lists.ubuntu.com/archives/ubuntu-announce/2025-April/000311.html)! \o/
- Helped [open the 25.10 Questing Quokka archive](https://lists.ubuntu.com/archives/ubuntu-devel/2025-May/043348.html). Let the development begin!
- Jon, VP of Engineering, asked me to lead the Canonical Release team - that was definitely not something I saw coming. :)
- We're now doing Ubuntu monthly releases for the devel releases - I'll be the tech lead for the project.
- Preparing for the May sprints - too many new things and new responsibilities. :)

---

## Debian (E)LTS
{{< figure src="/images/debian-lts-small.png" >}}

[Debian Long Term Support (LTS)](https://www.freexian.com/en/services/debian-lts.html) is a project to extend the lifetime of all Debian stable releases to (at least) 5 years. Debian LTS is not handled by the Debian security team, but by a separate group of volunteers and companies interested in making it a success.  

And [Debian Extended LTS (ELTS)](https://deb.freexian.com/extended-lts) is its sister project, extending support to the stretch and jessie release (+2 years after LTS support).

This was my 67th month as a Debian LTS and 54th month as a Debian ELTS paid contributor.  
Due to DC25 bursary work, Ubuntu 25.04 release, and other travel bits, I only worked for 2.00 hours for LTS and 4.50 hours for ELTS.

I did the following things:

- [ELTS] Had already backported patches for [adminer](https://tracker.debian.org/pkg/adminer) for the following CVEs:   
  - [CVE-2023-45195](https://security-tracker.debian.org/tracker/CVE-2023-45195): a SSRF attack.
  - [CVE-2023-45196](https://security-tracker.debian.org/tracker/CVE-2023-45196): a denial of service attack.
  - Salsa repository: https://salsa.debian.org/lts-team/packages/adminer.
  - As the same CVEs are affected LTS, we decided to release for LTS first and then for ELTS but since I had no hours for LTS, I decided to do a bit more of testing for ELTS to make sure things don't regress in buster.
  - Will prepare LTS (and also s-p-u, sigh) updates this month and get back to ELTS thereafter.
- [LTS] Started to prepare the LTS update for adminer for the same CVEs as for ELTS:
  - [CVE-2023-45195](https://security-tracker.debian.org/tracker/CVE-2023-45195): a SSRF attack.
  - [CVE-2023-45196](https://security-tracker.debian.org/tracker/CVE-2023-45196): a denial of service attack.
  - Haven't fully backported the patch yet but this is what I intend to do for this month (now that I have hours :D).
- [LTS] Partially attended the LTS meeting on Jitsi. [Summary here](https://lists.debian.org/debian-lts/2025/04/msg00059.html).
  - "Partially" because I was fighting SSO auth issues with Jitsi. Looks like there were some upstream issues/activity and it was resulting in gateway crashes but all good now.
  - I was following the running notes and keeping up with things as much as I could. :)

---

Until next time.  
`:wq` for today.
