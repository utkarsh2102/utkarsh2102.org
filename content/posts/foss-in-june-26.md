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

## Debian (E)LTS
{{< figure src="/images/debian-lts-small.png" >}}

This month I have worked 15 hours
on [Debian Long Term Support (LTS)](https://www.freexian.com/lts/debian/)
and on its sister [Extended LTS](https://www.freexian.com/lts/extended/)
project and did the following things:

### Released Security Updates

- **node-lodash**: Prototype pollution and code injection during template compilation.
  - **[LTS]**: Fixed [CVE-2025-13465](https://security-tracker.debian.org/tracker/CVE-2025-13465), [CVE-2026-2950](https://security-tracker.debian.org/tracker/CVE-2026-2950), and [CVE-2026-4800](https://security-tracker.debian.org/tracker/CVE-2026-4800) via [**4.17.21+dfsg+~cs8.31.173-1+deb11u1**](https://tracker.debian.org/news/1770027/accepted-node-lodash-41721dfsgcs831173-1deb11u1-source-into-oldoldstable-security/) for bullseye. This has been released as [**DLA 4663-1**](https://www.debian.org/lts/security/2026/DLA-4663-1).
  - **[trixie]**: Filed the proposed-update ([#1141450](https://bugs.debian.org/cgi-bin/bugreport.cgi?bug=1141450)) and uploaded the fix.
  - **[bookworm]**: Filed the proposed-update ([#1141449](https://bugs.debian.org/cgi-bin/bugreport.cgi?bug=1141449)) but it was closed; will release the DLA next month (in July).

- **openvpn**: Multiple vulnerabilities leading to Denial of Service.
  - **[LTS]**: Fixed [CVE-2026-11771](https://security-tracker.debian.org/tracker/CVE-2026-11771), [CVE-2026-12932](https://security-tracker.debian.org/tracker/CVE-2026-12932), [CVE-2026-12996](https://security-tracker.debian.org/tracker/CVE-2026-12996), [CVE-2026-13117](https://security-tracker.debian.org/tracker/CVE-2026-13117), [CVE-2026-13122](https://security-tracker.debian.org/tracker/CVE-2026-13122), and [CVE-2026-13698](https://security-tracker.debian.org/tracker/CVE-2026-13698) via **2.6.14-0+deb12u2** for bookworm. This has been released as [**DLA 4666-1**](https://www.debian.org/lts/security/2026/DLA-4666-1). The update itself was prepared by the maintainer; I helped prepare the paperwork.

### Work in Progress

- **php-phpseclib**: Affected by [CVE-2023-52892](https://security-tracker.debian.org/tracker/CVE-2023-52892) and [CVE-2026-32935](https://security-tracker.debian.org/tracker/CVE-2026-32935).
  - **[LTS]**: Continued to work on this and it should be released soon. Uploaded the work to debusine: https://debusine.debian.net/debian/developers/work-request/906743/. Will release the DLA in July.

### Other Activities

- **[LTS]** Emilio pointed out that the gst-plugins-ugly1.0 binaries were still not fully released, so I ran `dcut migrate` to fully release them. The DLA had gone out earlier.

- **[ELTS]** Did some more work on ruby-rack - a lot of new CVEs have opened up and, whilst I made some progress, Santiago let me know that ruby-rack is no longer supported and so it'll be removed from the `ela-needed` list.

- **[E/LTS]** Set up the security-tracker and a few other things on the new machine, and debugged the git repository size madness. Sent a summary [here](https://lists.debian.org/debian-lts/2026/07/msg00013.html).

- **[E/LTS]** Monitored discussions on mailing lists, IRC, and all the documentation updates.

- **[E/LTS]** Attended the monthly LTS meeting on Jitsi. [Meeting notes here](https://lists.debian.org/debian-lts/2026/06/msg00045.html).

---

Until next time.  
`:wq` for today.
