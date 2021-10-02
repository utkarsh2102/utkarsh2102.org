+++
date = "2021-10-01 11:11:11 +0530"
title = "FOSS Activites in September 2021"
slug = "foss-in-sept-21"
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

Here's my (twenty-fourth) monthly but brief update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 33rd month of actively contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March 2019 and a [DD](https://wiki.debian.org/DebianDeveloper) on Christmas '19! \o/

Just churning through the backlog this month. Ugh.

Anyway, I did the following stuff in Debian:

#### Uploads and bug fixes:

Hah, as a surprise, I did no uploads or bug fixes this month. :(

#### Other $things:

- Mentoring for newcomers.
- Moderation of -project mailing list.

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

This was my 8th month of actively contributing to [Ubuntu](https://ubuntu.com/about).
Now that I've joined [Canonical to work on Ubuntu full-time](https://utkarsh2102.com/posts/hello-canonical/), there's a bunch of things I do! \o/

I mostly worked on different things, I guess.

I was too lazy to maintain a list of things I worked on so there's
no concrete list atm. Maybe I'll get back to this section later or
will start to list stuff from next year onward, as I was doing before. :D

---

## Debian (E)LTS
{{< figure src="/images/debian-lts-small.png" >}}

[Debian Long Term Support (LTS)](https://www.freexian.com/en/services/debian-lts.html) is a project to extend the lifetime of all Debian stable releases to (at least) 5 years. Debian LTS is not handled by the Debian security team, but by a separate group of volunteers and companies interested in making it a success.  

And [Debian Extended LTS (ELTS)](https://deb.freexian.com/extended-lts) is its sister project, extending support to the Jessie release (+2 years after LTS support).

This was my twenty-fourth month as a Debian LTS and twelfth month as a Debian ELTS paid contributor.  
I was assigned 24.75 hours for LTS and 40.00 hours for ELTS and worked on the following things:  
(however, I worked for 6.75h more on ELTS work, thereby, making a total of 46.75h)

#### LTS CVE Fixes and Announcements:

- Issued [DLA 2751-1](), fixing [CVE-2021-3449](https://security-tracker.debian.org/tracker/CVE-2021-3449), for [postgresql-9.6](https://tracker.debian.org/pkg/postgresql-9.6).  
  For Debian 9 stretch, these problems have been fixed in version 3.20181128.1~deb9u1.  
  However, please note that the update was prepped by the maintainer, Christoph Berg. \o/
- Issued [DLA 2777-1](), fixing [CVE-2020-19131](https://security-tracker.debian.org/tracker/CVE-2020-19131) and [CVE-2020-19144](https://security-tracker.debian.org/tracker/CVE-2020-19144), for [tiff](https://tracker.debian.org/pkg/tiff).  
  For Debian 9 stretch, these problems have been fixed in version 4.0.8-2+deb9u7.
- Still discussing salt DLA/DSA uploads with Fredrico, Damien, and the maintainer.  
  I reviewed the patch and it looks good but we've been having build issues on buster, so have postponed the update/upload for a bit. Will need a fresh look.
- Philipp Hann raised the issue for incomplete uploads of amd64-microcode, where the binaries haven't been pusblished yet.  
  I took a look and that seems to be a valid bug/report, I've further discussed with the buildd admins and the security team to see what we can do here.
- Raphael Hertzog raised a bug for debian-archive-keyring, which needs an update prepped for stretch.  
  I've been looking at the same and mildly prepped the update, but still work-in-progress.

#### ELTS CVE Fixes and Announcements:

- Issued [ELA 486-1](), fixing [CVE-2021-3185](https://security-tracker.debian.org/tracker/CVE-2021-3185), for [gst-plugins-bad0.10](https://tracker.debian.org/pkg/gst-plugins-bad0.10).  
  For Debian 8 jessie, these problems have been fixed in version 0.10.23-7.4+deb8u5.
- Issued [ELA 492-1](), fixing [CVE-2020-19131](https://security-tracker.debian.org/tracker/CVE-2020-19131) and [CVE-2020-19144](https://security-tracker.debian.org/tracker/CVE-2020-19144), for [tiff](https://tracker.debian.org/pkg/tiff).  
  For Debian 8 jessie, these problems have been fixed in version 4.0.3-12.3+deb8u12.
- Issued [ELA 495-1](), fixing [CVE-2021-31799](https://security-tracker.debian.org/tracker/CVE-2021-31799), [CVE-2021-31810](https://security-tracker.debian.org/tracker/CVE-2021-31810), and [CVE-2021-32066](https://security-tracker.debian.org/tracker/CVE-2021-32066), for [ruby2.1](https://tracker.debian.org/pkg/ruby2.1).  
  For Debian 8 jessie, these problems have been fixed in version 2.1.5-2+deb8u12.
- Discussed the libjdom1-java regression plausiblity with the security team, where the last uploader forgot to include a regression fix and thus warrants a regression upload now.  
  Working on checking the severity w/ upstream to see how urgent it is.
- Worked on jsoup intensively. Discussed w/ upstream via [issue #1627](https://github.com/jhy/jsoup/issues/1627).  
  Further checked how plausible this is and discussed this on the internal list w/ Markus and Raphael.
- Whilst a separate section (below), it's also worth noting here that this time's front-desk triages had to be precise as there were really close calls to be made w.r.t. to the decisions made by the Debian's security and Ubuntu's security team.  
  More on that below.

#### Other (E)LTS Work:

- Front-desk duty from 30-08 until 05-09 and 27-09 to 03-10 for both LTS and ELTS.
- Triaged [ffmpeg](https://tracker.debian.org/pkg/ffmpeg),
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
[]
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
