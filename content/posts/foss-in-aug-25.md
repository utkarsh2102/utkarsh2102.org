+++
date = "2025-08-30 11:11:11 +0530"
title = "FOSS Activites in August 2025"
slug = "foss-in-aug-25"
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

Debian 13 was released! Woot!

Whilst I didn't get a chance to do much, here's still a few things that I worked on:

- Helped Anshul with Golang 1.25 packaging and upload.
- Assited Anshul in fixing Golang bugs in the stable release via a -pu.
- Mentoring for newcomers.
- Moderation of -project mailing list.

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

I joined [Canonical to work on Ubuntu full-time](https://utkarsh2102.org/posts/hello-canonical/) back in February 2021.

Whilst I can't give a full, detailed list of things I did, here's a quick TL;DR of what I did:

- [Released Questing snapshot 4](https://lists.ubuntu.com/archives/ubuntu-devel/2025-August/043431.html)! \o/
- Prepared for 25.10 Beta, held weekly release syncs, et al.
- Granted FFe and triaged a bunch of other bugs from both, Release team and Archive Admin POV. :)
- Got a recognition award for helping Chlo with Google Guest Agent packages.
- Preparing for the a round of internal review, 360s, and trying to not be sick. :)

---

## Debian (E)LTS
{{< figure src="/images/debian-lts-small.png" >}}

[Debian Long Term Support (LTS)](https://www.freexian.com/en/services/debian-lts.html) is a project to extend the lifetime of all Debian stable releases to (at least) 5 years. Debian LTS is not handled by the Debian security team, but by a separate group of volunteers and companies interested in making it a success.  

And [Debian Extended LTS (ELTS)](https://deb.freexian.com/extended-lts) is its sister project, extending support to the stretch and jessie release (+2 years after LTS support).

I only worked for 16.00 hours for LTS and 4.50 hours for ELTS and did the following things:

- [LTS] Prepared the LTS update for wordpress, bumping the package from 5.7.11 to 5.7.13.
  - Prepared an update for stable, too, and pinged Craig. Haven't heard yet.
  - Got incredibly sick so will carry on the coordination work and release the updates to all the releases. Everything's mostly ready and tested.
  - Gave Salvatore a quick heads up via IRC.
- [E/LTS] Frontdesk duty from 28th July to 04th August.
  - Triaged a bunch of packages and CVEs.
  - Raised an inconsistency about [issues being fixed in buster & bookworm but not in bullseye](https://lists.debian.org/debian-lts/2025/07/msg00017.html).
  - Also triaged some newly supported packages for ELTS.
- [E/LTS] Helped Daniel Leidert in showing him around as he did his first frontdesk rota. Yay! 🎉
  - We paired on an hour long meets call and discussed various toolings and workflows.
  - Pair-reviewed a few CVEs together.
  - Also discussed how to triage newly supported packages for ELTS, too!
- [LTS] Attended the monthly LTS meeting on Jitsi. [Summary here](https://lists.debian.org/debian-lts/2025/08/msg00042.html).
  - [ELTS] Raised questions about installing debusine on Ubuntu.
    - Still trying to play around to get a bit more comfortable before starting to do actual uploads there.
- [LTS] Helping a few folks - like assisting Lee to see if we have a reproducer for CVE-2025-27613 for git, et al.
- [Stable] Been working on fixing 2 packages: 
  - ruby-graphql: The Debian Security team asked to fix that via p-u so prepared a patch update.
  - ruby-saml: The update is finally ready but not tested yet - should be a quick one though.
  - Got incredibly sick and couldn't move things forward but will take care of the work in the following month.

---

Until next time.  
`:wq` for today.
