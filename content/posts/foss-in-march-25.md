+++
date = "2025-03-30 11:11:11 +0530"
title = "FOSS Activites in March 2025"
slug = "foss-in-march-25"
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

Here's my 66th monthly but brief update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 75th month of actively contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March 2019 and a [DD](https://wiki.debian.org/DebianDeveloper) on Christmas '19! \o/

There's a bunch of things I do, both, technical and non-technical. Here's what I did:

- Updating Rails to v7.2.2.1 for Trixie.
- Updating Redmine to v6.0.4 for Trixie.
- Kickstarting the bursary team for DC25.
- Mentoring for newcomers.
- Moderation of -project mailing list.

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

This was my 50th month of actively contributing to [Ubuntu](https://ubuntu.com/about).
Now that I joined [Canonical to work on Ubuntu full-time](https://utkarsh2102.org/posts/hello-canonical/), there's a bunch of things I do! \o/

I mostly worked on different things, I guess.

I was too lazy to maintain a list of things I worked on so there's
no concrete list atm. Maybe I'll get back to this section later or
will start to list stuff from the fall, as I was doing before. :D

---

## Debian (E)LTS
{{< figure src="/images/debian-lts-small.png" >}}

[Debian Long Term Support (LTS)](https://www.freexian.com/en/services/debian-lts.html) is a project to extend the lifetime of all Debian stable releases to (at least) 5 years. Debian LTS is not handled by the Debian security team, but by a separate group of volunteers and companies interested in making it a success.  

And [Debian Extended LTS (ELTS)](https://deb.freexian.com/extended-lts) is its sister project, extending support to the stretch and jessie release (+2 years after LTS support).

This was my 66th month as a Debian LTS and 53rd month as a Debian ELTS paid contributor.  
I worked for 15.00 hours for LTS and 7.50 hours for ELTS.

I did the following things:

- [ELTS] Worked on backporting patches for [adminer](https://tracker.debian.org/pkg/adminer).  
  - [CVE-2023-45195](https://security-tracker.debian.org/tracker/CVE-2023-45195): a SSRF attack.
  - [CVE-2023-45196](https://security-tracker.debian.org/tracker/CVE-2023-45196): a denial of service attack.
  - Salsa repository: https://salsa.debian.org/lts-team/packages/adminer.
  - Update has been prepared and partly tested. Will be released next month.
  - Will speak to FD for also fixing this for LTS.
- [E/LTS] Working on the musl fixes for bullseye. Taking it forward from where it was left off by Chris.
  - Co-ordiating with Santiago to see how to best get the reproducer to test the update.
  - Plan is to reproduce it myself but then reach out to Adrian if that doesn't work out.
  - Also makes sense to upload to LTS first, let it settle there, and then look at ELTS.
- [LTS] Attended the LTS meeting on IRC. [Summary here](https://meetbot.debian.net/debian-lts/2025/debian-lts.2025-03-27-14.00.html).
- [stable] Co-ordinated with the Security team to fix rails in bookworm via 2:6.1.7.10+dfsg-1~deb12u1.
  - Fixes: CVE-2023-28362, CVE-2023-38037, CVE-2024-26144, CVE-2024-28103, CVE-2024-41128, CVE-2024-47887, CVE-2024-47888, CVE-2024-47889, and CVE-2024-54133.
  - Released as [DSA 5881-1](https://lists.debian.org/debian-security-announce/2025/msg00043.html).
- [stable] Co-ordinated with the Security team to fix ruby-rack in bookworm via 2.2.13-1~deb12u1.
  - Fixes: CVE-2025-27610, CVE-2025-27111, and CVE-2025-25184.
  - Released as [DSA 5886-1](https://lists.debian.org/debian-security-announce/2025/msg00048.html).
- [stable] Partly co-ordinated with the Security team to fix ruby-saml in bookworm.

---

Until next time.  
`:wq` for today.
