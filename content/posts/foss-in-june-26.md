+++
date = "2026-06-30 11:11:11 +0530"
title = "FOSS Activities in June 2026"
slug = "foss-in-june-26"
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
  - This took most of my Debian time this month but we've been able to wrap that work now.
  - Got back to all the tickets on Zammad, too.
- Assisted a few folks in getting their patches submitted via Salsa.
- Mentoring for newcomers.
- Moderation of -project mailing list.

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

I joined [Canonical to work on Ubuntu full-time](https://utkarsh2102.org/posts/hello-canonical/) back in February 2021.

Whilst I can't give a full, detailed list of things I did, here's a quick TL;DR of what I did:

- Continued to push for infrastructure improvements:
  - Charming.
  - Artifact signing.
  - Reorganizing cdimage.
  - And so on.
- Successfully released [26.10 Snapshot 2](https://discourse.ubuntu.com/t/stonking-snapshot-2-released/84537)!
  - We landed a breaking change in the directory structure.
  - ...whihc had consequences on the rsync, being run by the sysadmins.
    - The 30 GB rsync failed because of the load on the system and it resulted in things blowing up. Yay. Stress-testing the shit out of our infra. :)
    - We got it back under control in the next few days but oh wow, what a journey to get there.
- Assisted a bunch of folks with my Archive Admin and Release team hats to:
  - Helped in archive opening tasks.
  - Promoting/demoting binaries to/from main.
  - Taking care of package removals and so on.
  - Reviewed the NEW queue.
- Reviewed quite a lot of MPs, specs, and other people's work.
- Mentoring, coaching, and leading the Release Management team.

---

Until next time.  
`:wq` for today.
