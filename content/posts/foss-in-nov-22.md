+++
date = "2022-11-30 11:11:11 +0530"
title = "FOSS Activites in November 2022"
slug = "foss-in-nov-22"
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

Here's my (thirty-eighth) monthly but brief update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 47th month of actively contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March 2019 and a [DD](https://wiki.debian.org/DebianDeveloper) on Christmas '19! \o/

There's a bunch of things I do, both, technical and non-technical. Here are the things I did this month:

#### Debian Uploads

- [tango](https://tracker.debian.org/pkg/tango) (9.3.4+dfsg1-2) - Fix FTBFS: configure: error; cf: [bug#1020056](https://bugs.debian.org/1020056).

#### Other $things:

- Sponsoring stuff for non-DDs.
- Mentoring for newcomers.
- Moderation of -project mailing list.

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

This was my 22nd month of actively contributing to [Ubuntu](https://ubuntu.com/about).
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

This was my thirty-eighth month as a Debian LTS and twenty-nine month as a Debian ELTS paid contributor.  
I worked for 41.00 hours for LTS and 30.25 hours for ELTS.

#### LTS CVE Fixes and Announcements:

- Issued [DLA 3187-1](https://lists.debian.org/debian-lts-announce/2022/11/msg00015.html), fixing [CVE-2021-36369](https://security-tracker.debian.org/tracker/CVE-2021-36369), for [dropbear](https://tracker.debian.org/pkg/dropbear).  
  For Debian 10 buster, these problems have been fixed in version 2018.76-5+deb10u2.
- Issued [DLA 3188-1](https://lists.debian.org/debian-lts-announce/2022/11/msg00014.html), fixing [CVE-2019-16167](https://security-tracker.debian.org/tracker/CVE-2019-16167), [CVE-2019-19725](https://security-tracker.debian.org/tracker/CVE-2019-19725), and [CVE-2022-39377](https://security-tracker.debian.org/tracker/CVE-2022-39377), for [sysstat](https://tracker.debian.org/pkg/sysstat).  
  For Debian 10 buster, these problems have been fixed in version 12.0.3-2+deb10u1.
- Issued [DLA 3189-1](https://lists.debian.org/debian-lts-announce/2022/11/msg00017.html) for a minor LTS version update of [postgresql-11](https://tracker.debian.org/pkg/postgresql-11).  
  For Debian 10 buster, the package has been updated to version 11.18-0+deb10u1.
- Issued [DLA 3215-1](https://lists.debian.org/debian-lts-announce/2022/12/msg00000.html), fixing [CVE-2022-3328](https://security-tracker.debian.org/tracker/CVE-2022-3328), for [snapd](https://tracker.debian.org/pkg/snapd).  
  For Debian 10 buster, these problems have been fixed in version 2.37.4-1+deb10u2.
- Issued [DLA 3216-1](https://lists.debian.org/debian-lts-announce/2022/12/msg00001.html), fixing [CVE-2022-41325](https://security-tracker.debian.org/tracker/CVE-2022-41325), for [vlc](https://tracker.debian.org/pkg/vlc).  
  For Debian 10 buster, these problems have been fixed in version 3.0.17.4-0+deb10u2.
- Issued [DLA 3217-1](https://lists.debian.org/debian-lts-announce/2022/12/msg00002.html), fixing [CVE-2022-46338](https://security-tracker.debian.org/tracker/CVE-2022-46338), for [g810-led](https://tracker.debian.org/pkg/g810-led).  
  For Debian 10 buster, these problems have been fixed in version 0.3.3-2+deb10u1.
- Issued [DLA 3218-1](https://lists.debian.org/debian-lts-announce/2022/12/msg00003.html), fixing [CVE-2022-41946](https://security-tracker.debian.org/tracker/CVE-2022-41946), for [libpgjava](https://tracker.debian.org/pkg/libpgjava).  
  For Debian 10 buster, these problems have been fixed in version 42.2.5-2+deb10u3.
- Issued [DLA 3220-1](https://lists.debian.org/debian-lts-announce/2022/12/msg00005.html) for a new upstream version update of [clamav](https://tracker.debian.org/pkg/clamav).  
  For Debian 10 buster, the package has been updated to version 0.103.7+dfsg-0+deb10u1.
- Started to look at other set of packages.

#### ELTS CVE Fixes and Announcements:

- Issued [ELA 731-1](https://www.freexian.com/lts/extended/updates/ela-731-1-sysstat/), fixing [CVE-2022-39377](https://security-tracker.debian.org/tracker/CVE-2022-39377), for [sysstat](https://tracker.debian.org/pkg/sysstat).  
  For Debian 9 stretch, these problems have been fixed in version 11.4.3-2+deb9u1.  
  For Debian 8 jessie, these problems have been fixed in version 11.0.1-1+deb8u1.
- Issued [ELA 749-1](https://www.freexian.com/lts/extended/updates/ela-749-1-vlc/), fixing [CVE-2022-41325](https://security-tracker.debian.org/tracker/CVE-2022-41325), for [vlc](https://tracker.debian.org/pkg/vlc).  
  For Debian 9 stretch, these problems have been fixed in version 3.0.17.4-0+deb9u2.
- Issued [ELA 750-1](https://www.freexian.com/lts/extended/updates/ela-750-1-clamav/) for a new upstream version update of [clamav](https://tracker.debian.org/pkg/clamav).  
  For Debian 9 stretch, the package has been updated to version 0.103.7+dfsg-0+deb9u1.
  For Debian 8 jessie, the package has been updated to version 0.103.7+dfsg-0+deb8u1.
- Started to look at other set of packages.

#### Other (E)LTS Work:

- Front desk duty from 21-11 until 27-11 for both, LTS and ELTS.
- Triaged [jqueryui](https://tracker.debian.org/pkg/jqueryui),
[open-vm-tools](https://tracker.debian.org/pkg/open-vm-tools),
[systemd](https://tracker.debian.org/pkg/systemd),
[ffmpeg](https://tracker.debian.org/pkg/ffmpeg),
[lava](https://tracker.debian.org/pkg/lava),
[pngcheck](https://tracker.debian.org/pkg/pngcheck),
[snapd](https://tracker.debian.org/pkg/snapd),
[vlc](https://tracker.debian.org/pkg/vlc),
[g810-led](https://tracker.debian.org/pkg/g810-led),
[libpgjava](https://tracker.debian.org/pkg/libpgjava),
[dropbear](https://tracker.debian.org/pkg/dropbear),
[python3.5](https://tracker.debian.org/pkg/python3.5),
[python3.4](https://tracker.debian.org/pkg/python3.4),
[clamav](https://tracker.debian.org/pkg/clamav),
[systat](https://tracker.debian.org/pkg/systat),
[postgresql-11](https://tracker.debian.org/pkg/postgresql-11), and
[mariadb-10.1](https://tracker.debian.org/pkg/mariadb-10.1).
- Marked CVE-2009-1143/open-vm-tools as postponed for buster, stretch and jessie.
- Marked CVE-2022-45873/systemd as not-affected in stretch and jessie.
- Marked CVE-2022-396{4,5}/ffmpeg as postponed for buster and stretch.
- Marked CVE-2022-45061/python3.{4,5} as postponed for stretch and jessie.
- Marked CVE-2022-31160/jqueryui as not-affected for jessie instead.
- Noted CVE-2022-45061/python3.4 to be marked as postponed; only things to fix is the armhf FTBFS.
- Auto EOL'd linux, libpgjava, nvidia-graphics-drivers, maradns, chromium, and glance for ELTS.
- Helped and assisted new contributors joining Freexian (LTS/ELTS/internally).
- Answered questions (& discussions) on IRC (#debian-lts and #debian-elts) and Matrix.
- Participated and helped fellow members with their queries via private mail and chat.
- General and other discussions on LTS private and [public mailing list](https://lists.debian.org/debian-lts/2022/11/threads.html).
- Attended the monthly meeting held on IRC on November 24th.

---

Until next time.  
`:wq` for today.
