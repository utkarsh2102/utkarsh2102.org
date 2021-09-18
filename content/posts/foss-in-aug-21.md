+++
date = "2021-09-01 11:11:11 +0530"
title = "FOSS Activites in August 2021"
slug = "foss-in-aug-21"
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

Here's my (twenty-third) monthly but brief update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 32nd month of actively contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March 2019 and a [DD](https://wiki.debian.org/DebianDeveloper) on Christmas '19! \o/

Tough month but I mostly spent on it churning through the immense backlog. But that
somewhat backfired and I have even more backlog than ever. :D

Anyway, I did the following stuff in Debian:

#### Uploads and bug fixes:

- [ruby3.0](https://tracker.debian.org/pkg/ruby3.0) (3.0.0-2) - Upload to unstable! \o/

#### Other $things:

- Mentoring for newcomers.
- Moderation of -project mailing list.

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

This was my 7th month of actively contributing to [Ubuntu](https://ubuntu.com/about).
Now that I've joined [Canonical to work on Ubuntu full-time](https://utkarsh2102.com/posts/hello-canonical/), there's a bunch of things I do! \o/

I mostly worked on different things, I guess. But mostly on packaging [keylime](https://github.com/utkarsh2102/python-keylime) and some Google Agents upload(s) and SRU(s). Also did a lot of reviewing, et al.

I was too lazy to maintain a list of things I worked on so there's no concrete list atm. Maybe I'll get back to this section later or will start to list stuff from next month onward, as I've been doing before. :D

---

## Debian (E)LTS
{{< figure src="/images/debian-lts-small.png" >}}

[Debian Long Term Support (LTS)](https://www.freexian.com/en/services/debian-lts.html) is a project to extend the lifetime of all Debian stable releases to (at least) 5 years. Debian LTS is not handled by the Debian security team, but by a separate group of volunteers and companies interested in making it a success.  

And [Debian Extended LTS (ELTS)](https://deb.freexian.com/extended-lts) is its sister project, extending support to the Jessie release (+2 years after LTS support).

This was my twenty-third month as a Debian LTS and eleventh month as a Debian ELTS paid contributor.  
I was assigned 23.75 hours for LTS and 40.00 hours for ELTS and worked on the following things:  
(however, I only worked for 23.75h on ELTS work, thereby, carrying the rest to next month)

#### LTS CVE Fixes and Announcements:

- Issued [DLA 2743-1](https://lists.debian.org/debian-lts-announce/2021/08/msg00019.html), fixing [CVE-2017-5715](https://security-tracker.debian.org/tracker/CVE-2017-5715), for [amd64-microcode](https://tracker.debian.org/pkg/amd64-microcode).  
  For Debian 9 stretch, these problems have been fixed in version 3.20181128.1~deb9u1.
- Issued [DLA 2744-1](https://lists.debian.org/debian-lts-announce/2021/08/msg00021.html), fixing the [versioning issue](https://bugs.debian.org/991808), for [usermode](https://tracker.debian.org/pkg/usermode).  
  For Debian 9 stretch, these problems have been fixed in version 1.109-1+deb9u1.
- Issued [DLA 2750-1](https://lists.debian.org/debian-lts-announce/2021/08/msg00028.html), fixing [CVE-2019-20421](https://security-tracker.debian.org/tracker/CVE-2019-20421), [CVE-2021-3482](https://security-tracker.debian.org/tracker/CVE-2021-3482), [CVE-2021-29457](https://security-tracker.debian.org/tracker/CVE-2021-29457), [CVE-2021-29473](https://security-tracker.debian.org/tracker/CVE-2021-29473), [CVE-2021-31291](https://security-tracker.debian.org/tracker/CVE-2021-31291), and [CVE-2021-31292](https://security-tracker.debian.org/tracker/CVE-2021-31292), for [exiv2](https://tracker.debian.org/pkg/exiv2).  
  For Debian 9 stretch, these problems have been fixed in version 0.25-3.1+deb9u3.

#### ELTS CVE Fixes and Announcements:

- Issued [ELA 479-1](https://deb.freexian.com/extended-lts/updates/ela-479-1-exiv2/), fixing [CVE-2019-20421](https://security-tracker.debian.org/tracker/CVE-2019-20421), [CVE-2021-3482](https://security-tracker.debian.org/tracker/CVE-2021-3482), [CVE-2021-29457](https://security-tracker.debian.org/tracker/CVE-2021-29457), [CVE-2021-29473](https://security-tracker.debian.org/tracker/CVE-2021-29473), [CVE-2021-31291](https://security-tracker.debian.org/tracker/CVE-2021-31291), and [CVE-2021-31292](https://security-tracker.debian.org/tracker/CVE-2021-31292), for [exiv2](https://tracker.debian.org/pkg/exiv2).  
  For Debian 8 jessie, these problems have been fixed in version 0.24-4.1+deb8u6.
- Noticed that there's a fallout of CVE-2021-3185, where an update was issued for gst-plugins-bad1.0, however, not for gst-plugins-bad0.10.  
  Thanks to Sylvain's script, this came up and I prepped an update for that.
- Started to work on libjdom1-java's regression.

#### Other (E)LTS Work:

- Front-desk duty from 26-07 until 01-08 and from 30-08 until 05-09 for both LTS and ELTS.
- Triaged [haproxy](https://tracker.debian.org/pkg/haproxy),
[ntfs-3g](https://tracker.debian.org/pkg/ntfs-3g), and
[cyrus-imapd](https://tracker.debian.org/pkg/cyrus-imapd), and
[exiv2](https://tracker.debian.org/pkg/exiv2),
[ffmpeg](https://tracker.debian.org/pkg/ffmpeg),
[git](https://tracker.debian.org/pkg/git),
[gpac](https://tracker.debian.org/pkg/gpac),
[inetutils](https://tracker.debian.org/pkg/inetutils),
[mc](https://tracker.debian.org/pkg/mc),
[modsecurity-crs](https://tracker.debian.org/pkg/modsecurity-crs),
[node-object-path](https://tracker.debian.org/pkg/node-object-path),
[php-pear](https://tracker.debian.org/pkg/php-pear),
[systemd-cron](https://tracker.debian.org/pkg/systemd-cron),
[node-tar](https://tracker.debian.org/pkg/node-tar),
[ruby2.3](https://tracker.debian.org/pkg/ruby2.3),
[gst-plugins-bad0.10](https://tracker.debian.org/pkg/gst-plugins-bad0.10),
[jsoup](https://tracker.debian.org/pkg/jsoup),
[libxstream-java](https://tracker.debian.org/pkg/libxstream-java),
[qemu](https://tracker.debian.org/pkg/qemu),
[tomcat7](https://tracker.debian.org/pkg/tomcat7),
[ruby2.1](https://tracker.debian.org/pkg/ruby2.1),
[prototypejs](https://tracker.debian.org/pkg/prototypejs),
[pillow](https://tracker.debian.org/pkg/pillow),
[cpio](https://tracker.debian.org/pkg/cpio), and
[qtbase-opensource-src](https://tracker.debian.org/pkg/qtbase-opensource-src), and
[amd64-microcode](https://tracker.debian.org/pkg/amd64-microcode).
- Mark CVE-2021-39240/haproxy as not-affected for stretch and jessie.
- Mark CVE-2021-39241/haproxy as not-affected for stretch and jessie.
- Mark CVE-2021-39242/haproxy as not-affected for stretch and jessie.
- Mark CVE-2021-33582/cyrus-imapd as no-dsa for stretch.
- Mark CVE-2020-18771/exiv2 as no-dsa for exiv2 for stretch.
- Mark CVE-2020-18899/exiv2 as no-dsa for exiv2 for stretch.
- Mark CVE-2021-38171/ffmpeg as postponed for stretch.
- Mark CVE-2021-40330/git as no-dsa for stretch and jessie.
- Mark CVE-2020-19481/gpac as ignored for stretch.
- Mark CVE-2021-40491/inetutils as no-dsa for stretch.
- Mark CVE-2021-36370/mc as no-dsa for stretch and jessie.
- Mark CVE-2021-35368/modsecurity-crs as no-dsa for stretch.
- Mark CVE-2021-23434/node-object-path as end-of-life for stretch.
- Mark CVE-2021-32610/php-pear as no-dsa for stretch.
- Mark CVE-2017-9525/systemd-cron as no-dsa for stretch.
- Mark CVE-2021-37701/node-tar as end-of-life for stretch.
- Mark CVE-2021-37712/node-tar as end-of-life in stretch.
- Mark CVE-2021-3750/qemu as postponsed for jessie.
- Mark CVE-2021-27511/prototypejs as postponsed for jessie.
- Mark CVE-2021-23437/pillow as postponed for stretch and jessie.
- Auto EOL'ed gpac, cacti, openscad, cgal, cyrus-imapd-2.4, libsolv, mosquitto, atomicparsley, gtkpod, node-tar, libapache2-mod-auth-openidc, neutron, inetutils and linux for jessie.
- Drop cpio from ela-needed; open issues don't warrant an ELA.
- Attended monthly Debian LTS meeting.
- Answered questions (& discussions) on IRC (#debian-lts and #debian-elts).
- General and other discussions on LTS private and [public mailing list](https://lists.debian.org/debian-lts/2021/08/threads.html).

---

Until next time.  
`:wq` for today.
