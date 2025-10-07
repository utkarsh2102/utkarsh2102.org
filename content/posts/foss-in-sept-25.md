+++
date = "2025-09-30 11:11:11 +0530"
title = "FOSS Activites in September 2025"
slug = "foss-in-sept-25"
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

- Helped sponsor a patch for net-tools for Helge.
 - https://salsa.debian.org/debian/net-tools/-/merge_requests/5.
- Assited Anshul in his interest to do a Go 1.25 transition.
- Mentoring for newcomers.
- Moderation of -project mailing list.

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

I joined [Canonical to work on Ubuntu full-time](https://utkarsh2102.org/posts/hello-canonical/) back in February 2021.

Whilst I can't give a full, detailed list of things I did, here's a quick TL;DR of what I did:

- Successfully and timely [released 25.10 (Questing Quokka) Beta](https://lists.ubuntu.com/archives/ubuntu-announce/2025-September/000316.html)! \o/
- Continued to hold weekly release syncs, et al.
- Granted FFe and triaged a bunch of other bugs from both, Release team and Archive Admin POV. :)
- 360s were fab - I was a peak performer again. Yay!
- Preparing for the 25.10 Release sprints in London and then the Summit.
- Roadmap planning for the Release team.

---

## Debian (E)LTS
{{< figure src="/images/debian-lts-small.png" >}}

This month I have worked 16.50 hours on [Debian Long Term Support (LTS)](https://www.freexian.com/lts/debian/) and
05.50 hours on its sister [Extended LTS](https://www.freexian.com/lts/extended/) project and did the following things:

- [E/LTS] Frontdesk duty from 22nd September to 28th September.
  - Triaged lemonldap-ng, ghostscript, dovecot, node-ip, webkit2gtk, wpewebkit, libscram-java, keras, openbabel, gegl, tiff, zookeeper, squid, ogre-1.12, mapserver, ruby-rack.
  - Auto-EOL'd a few packages.
  - Also circled back on previously opened ticket for supported packages for ELTS.
  - Partially reviewed and added comment on [Emilio's MP](https://gitlab.com/freexian/services/deblts-team/debian-lts/-/merge_requests/64).
  - Re-visited an old thread (in order to fully close it) about issues being fixed in buster & bookworm but not in bullseye. And brought it up in the LTS meeting, too.

- [LTS] Partook in some internal discussions about introducing support for handling severity of CVEs, et al.
  - Santiago had asked for an input from people doing FD so spent some time reflecting on his proposal and getting back with thoughts and suggestions.

- [LTS] Helped Lee with testing gitk and git-gui aspects of his git update.

- [LTS] Attended the monthly LTS meeting on IRC. [Summary here](https://meetbot.debian.net/debian-lts/2025/debian-lts.2025-09-25-14.00.html).
  - It was also followed by a 40-minute discussion of technical questions/reviews/discussions - which in my opinion was pretty helpful. :)

- [LTS] Prepared the LTS update for wordpress, bumping the package from 5.7.11 to 5.7.13.
  - Prepared an update for stable, Craig approved. Was waiting on the Security team's +1 to upload.
  - Now we've waited enough that we have new CVEs. Oh well.

- [ELTS] Finally setup debusine for ELTS uploads.
  - Since I use Ubuntu, this required installing debusine* from bookworm-backport but that required Python 3.11.
  - So I had to upgrade from Jammy (22.04) to Noble (24.04) - which was anyway pending.. :)
  - And then followed the docs to configure it. \o/

- [E/LTS] Started working on new ruby-rack CVE.

---

Until next time.  
`:wq` for today.
