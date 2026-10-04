+++
date = "2026-10-05 11:11:11 +0530"
title = "FOSS Activities in September 2026"
slug = "foss-in-sept-26"
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

Whilst I didn't have much time, here are still a few things that I worked on:

- Sponsored [ubuntu-dev-tools/0.214](https://tracker.debian.org/news/1798457/accepted-ubuntu-dev-tools-0214-source-into-unstable/) for Florent 'Skia' Jacquet, which updates `seeded-in-ubuntu` to use the new per-series indexer ([LP: #2160240](https://bugs.launchpad.net/bugs/2160240)).
- Assisted a few folks in getting their patches submitted via Salsa.
- Mentoring for newcomers.
- Moderation of -project mailing list.

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

I joined [Canonical to work on Ubuntu full-time](https://utkarsh2102.org/posts/hello-canonical/) back in February 2021.

- With 26.10 in Feature Freeze, wore my Release team hat to:
  - Review and approve a bunch of Feature Freeze Exceptions, including the Go 1.27 transition, Qt 6.11.2, rust-coreutils 0.12.0, devscripts 2.6.12, kdump-tools moving to dracut, and a few GCE packages.
  - Point linux-entra-sso to the SRU team, as it didn't need an FFe at all, and milestone a couple of bugs for 26.10.
- Continued to push for infrastructure improvements:
  - Made ubuntu-cdimage more resilient to Launchpad hiccups ([MP](https://code.launchpad.net/~utkarsh/ubuntu-cdimage/+git/ubuntu-cdimage/+merge/511948)).
  - Taught `generate-freeze-block` in ubuntu-archive-tools a couple of new options (`--skip-update` and `--series`) and better error handling ([MP](https://code.launchpad.net/~utkarsh/ubuntu-archive-tools/+git/ubuntu-archive-tools/+merge/511844)).
  - Bumped the arm64 generic non-cloud image to 4.5G in livecd-rootfs and uploaded it as [26.10.16](https://launchpad.net/ubuntu/+source/livecd-rootfs/26.10.16); also sponsored the follow-up [26.10.17](https://launchpad.net/ubuntu/+source/livecd-rootfs/26.10.17) for Chloé.
- Sponsored [aevol/9.4.0-2ubuntu1](https://launchpad.net/ubuntu/+source/aevol/9.4.0-2ubuntu1) for Matthieu, fixing an FTBFS with GCC 15's LTO ([LP: #2167811](https://bugs.launchpad.net/bugs/2167811)).
- Reviewed quite a lot of MPs - britney hints, meta-release, ubuntu-release-tools, ubuntu-archive-tools, ubuntu-cdimage, livecd-rootfs, ubuntu-seeds, and so on.
- Enabled [upgrades to 26.04 LTS](https://discourse.ubuntu.com/t/upgrades-from-ubuntu-24-04-lts-to-ubuntu-26-04-1-lts-now-enabled/88502).
- Released 26.10 Beta and [announced it on Discourse](https://discourse.ubuntu.com/t/ubuntu-26-10-stonking-stingray-beta-released/88662).
- Did Archive Admin, DMB, and Release team duties as usual.

---

Until next time.  
`:wq` for today.
