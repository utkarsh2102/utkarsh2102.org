+++
date = "2023-12-30 11:11:11 +0530"
title = "FOSS Activites in December 2023"
slug = "foss-in-dec-23"
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

Here's my (fifty-first) monthly but brief update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 60th month of actively contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March 2019 and a [DD](https://wiki.debian.org/DebianDeveloper) on Christmas '19! \o/

There's a bunch of things I do, both, technical and non-technical. Here's what I did:

- Some sync up w/ DC24 team, gearing up for DC24 prep. \o/
- Mentoring for newcomers.
- Moderation of -project mailing list.

A huge thanks to Freexian for sponsoring my Debian work. :D

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

This was my 35th month of actively contributing to [Ubuntu](https://ubuntu.com/about).
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

This was my fifty-first month as a Debian LTS and thirty-eighth month as a Debian ELTS paid contributor.  
I worked for 18.75 hours for LTS and 23.25 hours for ELTS.

I did the following things:

- LTS & ELTS frontdesk from 11-12 to 17-12.
- Triaged [haproxy](https://tracker.debian.org/pkg/haproxy),
[ghostscript](https://tracker.debian.org/pkg/ghostscript),
[jq](https://tracker.debian.org/pkg/jq),
[libreoffice](https://tracker.debian.org/pkg/libreoffice),
[m2crypto](https://tracker.debian.org/pkg/m2crypto),
[python-cryptography](https://tracker.debian.org/pkg/python-cryptography),
[tar](https://tracker.debian.org/pkg/tar),
[espeak-ng](https://tracker.debian.org/pkg/espeak-ng),
[gnome-control-center](https://tracker.debian.org/pkg/gnome-control-center),
[slurm-llnl](https://tracker.debian.org/pkg/slurm-llnl),
[tor](https://tracker.debian.org/pkg/tor),
[budgie-extras](https://tracker.debian.org/pkg/budgie-extras),
[ncurses](https://tracker.debian.org/pkg/ncurses),
[shiro](https://tracker.debian.org/pkg/shiro),
[virtuoso-opensource](https://tracker.debian.org/pkg/virtuoso-opensource),
[kde4libs](https://tracker.debian.org/pkg/kde4libs), and
[zfs-linux](https://tracker.debian.org/pkg/zfs-linux).
- Marked CVE-2023-46751/ghostscript as not-affected for stretch and jessie.
- Marked CVE-2023-49355/jq as not-affected for stretch and jessie.
- Marked CVE-2023-50246/jq as not-affected for stretch and jessie.
- Marked CVE-2023-50268/jq as not-affected for stretch and jessie.
- Marked CVE-2023-50781/m2crypto as no-dsa for buster, stretch, and jessie.
- Marked CVE-2023-50782/python-cryptography as no-dsa for buster, stretch, and jessie.
- Marked CVE-2023-39804/tar as no-dsa for buster, stretch, and jessie.
- Marked CVE-2023-4999{0-5}/espeak-ng as no-dsa for buster and stretch.
- Marked CVE-2023-5616/gnome-control-center as no-dsa for stretch.
- Marked slurm-llnl CVEs as end-of-life for buster.
- Marked TEMP-0000000-7CC552/tor as end-of-life for buster.
- Marked CVE-2023-4934{2-6}/budgie-extras as no-dsa for buster and stretch.
- Marked CVE-2023-50495/ncurses as no-dsa for buster.
- Marked CVE-2023-46750/shiro as no-dsa for buster.
- Marked CVE-2023-489{45-52}/virtuoso-opensource as no-dsa for buster.
- Auto EOL'd capnproto, gpac, radare2, minizip, gimp-dds, libde265, strongswan, cargo, bouncycastle, linux, firefox-esr, thunderbird, gnutls28, gnome-control-center, chromium, tinyxml, asterisk, glpi, shiro, xen, slurm-llnl, wordpress, and derby.
- Worked on some distro-info-data updates for sid. Coordination w/ Stefano for E/LTS is still needed.
- Worked on zfs-linux and kde4libs partly. DLA and ELA to go out soon.
- Partook in various discussions about ELTS packages and their support w/ Santiago and Roberto, and others, during the Freexian sprints.
- Answered questions (& discussions) on IRC (#debian-lts and #debian-elts) and Matrix.
- Participated and helped fellow members with their queries.
- General and other discussions on LTS private and [public mailing list](https://lists.debian.org/debian-lts/2023/12/threads.html).
- Attended the monthly LTS meeting.

---

Until next time.  
`:wq` for today.
