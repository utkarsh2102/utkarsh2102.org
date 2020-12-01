+++
date = "2020-12-01 16:00:00 +0530"
title = "FOSS Activites in November 2020"
slug = "foss-in-nov-20"
images = [
    "/images/debian-logo-small.png",
    "/images/debian_ruby.png",
    "/images/ruby-logo-small.png",
    "/images/debian-lts-small.png",
    "/images/computing.jpg"
]
tags = [
    "debian",
    "monthly",
]
categories = [
    "debian",
    "open-source",
]
+++

Here's my (fourteenth) monthly update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 23rd month of contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March last year and a [DD](https://wiki.debian.org/DebianDeveloper) last Christmas! \o/

Apart from doing a bunch of activities like attending KubeCon + RubyConf (blog to follow!), et al and simultaneously giving
my undergrad exams, I did (relatively) more work than I had really anticipated!

Here are the following things I did in Debian this month:

#### Uploads and bug fixes:

- [slingshot-clojure](https://tracker.debian.org/pkg/slingshot-clojure) (0.12.2-3) - Fix for [bug #891311](https://bugs.debian.org/891311).
- [clj-stacktrace-clojure](https://tracker.debian.org/pkg/clj-stacktrace-clojure) (0.2.7-1) - New upstream version, v0.2.7, fixing [bug #852249](https://bugs.debian.org/852249).
- [golang-github-xo-terminfo](https://tracker.debian.org/pkg/golang-github-xo-terminfo) (0.0~git20200218.454e5b6-2) - New package + source-only upload.
- [golang-github-zyedidia-tcell](https://tracker.debian.org/pkg/golang-github-zyedidia-tcell) (2.0.6-1) - New upstream version, v2.0.6.
- [golang-github-zyedidia-clipboard](https://tracker.debian.org/pkg/golang-github-zyedidia-clipboard) (1.0.3-1) - New upstream version, 1.0.3.
- [micro](https://tracker.debian.org/pkg/micro) (2.0.8-1) - New upstream version, v2.0.8. Finally! \o/
- [ruby-zeitwerk](https://tracker.debian.org/pkg/ruby-zeitwerk) (2.4.2-1) - New upstream version, v2.4.2.

#### Other $things:

- Attended the Debian Ruby team meeting.
- Mentoring for newcomers.
- FTP Trainee reviewing.
- Moderation of -project mailing list.
- Sponsored `phpmyadmin` for William and `libexif` for Hugh.

---

## Debian (E)LTS
{{< figure src="/images/debian-lts-small.png" >}}

[Debian Long Term Support (LTS)](https://www.freexian.com/en/services/debian-lts.html) is a project to extend the lifetime of all Debian stable releases to (at least) 5 years. Debian LTS is not handled by the Debian security team, but by a separate group of volunteers and companies interested in making it a success.  

And [Debian Extended LTS (ELTS)](https://deb.freexian.com/extended-lts) is its sister project, extending support to the Jessie release (+2 years after LTS support).

This was my fourteenth month as a Debian LTS and fourth month as a Debian ELTS paid contributor.  
I was assigned 22.75 hours for LTS and 45.00 hours for ELTS and worked on the following things:  
(for ELTS, I worked for 5.25 hours last month, so I had to work for 39.75 (+1 extra) hours this month)  
(also, I did over-work by 5.00 hours for LTS this month, but I'll re-compensate it later to avoid so much fuss!)

#### LTS CVE Fixes and Announcements:

- Issued [DLA 2425-1](https://lists.debian.org/debian-lts-announce/2020/11/msg00000.html), fixing [CVE-2020-25692](https://security-tracker.debian.org/tracker/CVE-2020-25692), for [openldap](https://tracker.debian.org/pkg/openldap).  
  For Debian 9 Stretch, these problems have been fixed in version 2.4.44+dfsg-5+deb9u5.
- Issued [DLA 2427-1](https://lists.debian.org/debian-lts-announce/2020/11/msg00001.html), fixing [CVE-2020-14355](https://security-tracker.debian.org/tracker/CVE-2020-14355), for [spice](https://tracker.debian.org/pkg/spice).  
  For Debian 9 Stretch, these problems have been fixed in version 0.12.8-2.1+deb9u4.
- Issued [DLA 2428-1](https://lists.debian.org/debian-lts-announce/2020/11/msg00002.html), fixing [CVE-2020-14355](https://security-tracker.debian.org/tracker/CVE-2020-14355), for [spice-gtk](https://tracker.debian.org/pkg/spice-gtk).  
  For Debian 9 Stretch, these problems have been fixed in version 0.33-3.3+deb9u2.
- Issued [DLA 2429-1](https://lists.debian.org/debian-lts-announce/2020/11/msg00004.html), fixing [CVE-2020-28032](https://security-tracker.debian.org/tracker/CVE-2020-28032), [CVE-2020-28033](https://security-tracker.debian.org/tracker/CVE-2020-28033), [CVE-2020-28034](https://security-tracker.debian.org/tracker/CVE-2020-28034), [CVE-2020-28035](https://security-tracker.debian.org/tracker/CVE-2020-28035), [CVE-2020-28036](https://security-tracker.debian.org/tracker/CVE-2020-28036), [CVE-2020-28037](https://security-tracker.debian.org/tracker/CVE-2020-28037), [CVE-2020-28038](https://security-tracker.debian.org/tracker/CVE-2020-28038), [CVE-2020-28039](https://security-tracker.debian.org/tracker/CVE-2020-28039), and [CVE-2020-28040](https://security-tracker.debian.org/tracker/CVE-2020-28040), for [wordpress](https://tracker.debian.org/pkg/wordpress).  
  For Debian 9 Stretch, these problems have been fixed in version 4.7.19+dfsg-1+deb9u1.
- Issued [DLA 2430-1](https://lists.debian.org/debian-lts-announce/2020/11/msg00005.html), fixing [CVE-2020-15238](https://security-tracker.debian.org/tracker/CVE-2020-15238), for [blueman](https://tracker.debian.org/pkg/blueman).  
  For Debian 9 Stretch, these problems have been fixed in version 2.0.4-1+deb9u1.
- Issued [DLA 2439-1](https://lists.debian.org/debian-lts-announce/2020/11/msg00013.html), fixing [CVE-2020-0452](https://security-tracker.debian.org/tracker/CVE-2020-0452), for [libexif](https://tracker.debian.org/pkg/libexif).  
  For Debian 9 Stretch, these problems have been fixed in version 0.6.21-2+deb9u5.
- Issued [DLA 2443-1](https://lists.debian.org/debian-lts-announce/2020/11/msg00017.html), fixing [CVE-2020-15166](https://security-tracker.debian.org/tracker/CVE-2020-15166), for [zeromq3](https://tracker.debian.org/pkg/zeromq3).  
  For Debian 9 Stretch, these problems have been fixed in version 4.2.1-4+deb9u3.
- Issued [DLA 2444-1](https://lists.debian.org/debian-lts-announce/2020/11/msg00018.html), fixing [CVE-2020-8037](https://security-tracker.debian.org/tracker/CVE-2020-8037), for [tcpdump](https://tracker.debian.org/pkg/tcpdump).  
  For Debian 9 Stretch, these problems have been fixed in version 4.9.3-1~deb9u2.

#### ELTS CVE Fixes and Announcements:

- Issued [ELA 306-1](https://deb.freexian.com/extended-lts/updates/ela-306-1-openldap/), fixing [CVE-2020-25692](https://security-tracker.debian.org/tracker/CVE-2020-25692), for [openldap](https://tracker.debian.org/pkg/openldap).  
  For Debian 8 Jessie, these problems have been fixed in version 2.4.40+dfsg-1+deb8u7.
- Issued [ELA 310-1](https://deb.freexian.com/extended-lts/updates/ela-310-1-libexif/), fixing [CVE-2020-0452](https://security-tracker.debian.org/tracker/CVE-2020-0452), for [libexif](https://tracker.debian.org/pkg/libexif).  
  For Debian 8 Jessie, these problems have been fixed in version 0.6.21-2+deb8u5.
- Issued [ELA 311-1](https://deb.freexian.com/extended-lts/updates/ela-311-1-tcpdump/), fixing [CVE-2020-8037](https://security-tracker.debian.org/tracker/CVE-2020-8037), for [tcpdump](https://tracker.debian.org/pkg/tcpdump).  
  For Debian 8 Jessie, these problems have been fixed in version 4.9.3-1~deb8u2.
- Issued [ELA 312-1](https://deb.freexian.com/extended-lts/updates/ela-312-1-tzdata/), backporting a new upstream release, 2020d, for [tzdata](https://tracker.debian.org/pkg/tzdata).  
  For Debian 8 Jessie, these problems have been fixed in version 2020d-0+deb8u1.
- Issued [ELA 313-1](https://deb.freexian.com/extended-lts/updates/ela-313-1-zeromq3/), fixing [CVE-2020-15166](https://security-tracker.debian.org/tracker/CVE-2020-15166), for [zeromq3](https://tracker.debian.org/pkg/zeromq3).  
  For Debian 8 Jessie, these problems have been fixed in version 4.0.5+dfsg-2+deb8u3.
- Prepared a debdiff for lxml (3.4.0-1+deb8u2) upload, which Emilio completed and rolled out later.

#### Other (E)LTS Work:

- Front-desk duty from 26-10 until 01-10 and from 23-11 until 29-11 for both LTS and ELTS.
- Triaged [openldap](https://tracker.debian.org/pkg/openldap),
[python-cryptography](https://tracker.debian.org/pkg/python-cryptography),
[motion](https://tracker.debian.org/pkg/motion),
[nvidia-cuda-toolkit](https://tracker.debian.org/pkg/nvidia-cuda-toolkit),
[samba](https://tracker.debian.org/pkg/samba),
[lxml](https://tracker.debian.org/pkg/lxml),
[highlight.js](https://tracker.debian.org/pkg/highlight.js),
[imagemagick](https://tracker.debian.org/pkg/imagemagick),
[mongodb](https://tracker.debian.org/pkg/mongodb),
[poppler](https://tracker.debian.org/pkg/poppler),
[wordpress](https://tracker.debian.org/pkg/wordpress),
[raptor2](https://tracker.debian.org/pkg/raptor2), and
[blueman](https://tracker.debian.org/pkg/blueman).
- Marked CVE-2020-25659/python-cryptography as no-dsa for Stretch and Jessie.
- Marked CVE-2020-25713/raptor2 as postponed for Stretch and Jessie.
- Marked CVE-2020-27778/poppler as postponed for Stretch and Jessie.
- Marked CVE-2020-5991/nvidia-cuda-toolkit as ignored for Stretch.
- Marked CVE-2020-26566/motion as not-affected for Stretch.
- Marked CVE-2020-26237/highlight.js as postponed for Jessie.
- Auto EOL'ed libpam-tacplus, motion, blueman, openrc, webcit, wordpress, linux, nvidia-cuda-toolkit, spip, and wireshark for Jessie.
- Attended the sevent LTS meeting. Logs [here](http://meetbot.debian.net/debian-lts/2020/debian-lts.2020-11-26-14.59.html).
- General discussion on LTS private and [public mailing list](https://lists.debian.org/debian-lts/2020/11/threads.html).

---

Until next time.  
`:wq` for today.
