+++
date = "2022-02-01 11:11:11 +0530"
title = "FOSS Activites in January 2022"
slug = "foss-in-jan-22"
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

Here's my (twenty-eighth) monthly but brief update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 37th month of actively contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March 2019 and a [DD](https://wiki.debian.org/DebianDeveloper) on Christmas '19! \o/

Just churning through the backlog again this month. Ugh.

Anyway, I did the following stuff in Debian:

#### Uploads and bug fixes:

- [ruby2.5](https://tracker.debian.org/pkg/ruby2.5) (2.5.5-3+deb10u4) - Fixing CVE-2021-28965, CVE-2021-31799, CVE-2021-31810, CVE-2021-32066, Fixes: CVE-2021-41817, and CVE-2021-41819 for Buster.
- [mat2](https://tracker.debian.org/pkg/mat2) (0.12.2-1.1) - Add patch to fix AssertionError in test_libmat2, fixing bug #1002418.
- [ruby-fast-gettext](https://tracker.debian.org/pkg/ruby-fast-gettext) (2.0.3-2) - Add patch to fix FTBFS, fixing bug #1002103.
- [python-flask-marshmallow](https://tracker.debian.org/pkg/python-flask-marshmallow) (0.14.0-1) - New upstream version, v0.14.0, fixing bug #989269.
- [ruby-rack](https://tracker.debian.org/pkg/ruby-rack) (2.2.3-4) - Add patch to fix build and autopkgtest.
- [ruby2.7](https://tracker.debian.org/pkg/ruby2.7) (2.7.4-1+deb11u1) - Fixing CVE-2021-41816, CVE-2021-41817, and CVE-2021-41819 for Bullseye.

#### Other $things:

- Mentoring for newcomers.
- Moderation of -project mailing list.

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

This was my 12th month of actively contributing to [Ubuntu](https://ubuntu.com/about).
Now that I joined [Canonical to work on Ubuntu full-time](https://utkarsh2102.com/posts/hello-canonical/), there's a bunch of things I do! \o/

I mostly worked on different things, I guess.

I was too lazy to maintain a list of things I worked on so there's
no concrete list atm. Maybe I'll get back to this section later or
will start to list stuff from the fall, as I was doing before. :D

---

## Debian (E)LTS
{{< figure src="/images/debian-lts-small.png" >}}

[Debian Long Term Support (LTS)](https://www.freexian.com/en/services/debian-lts.html) is a project to extend the lifetime of all Debian stable releases to (at least) 5 years. Debian LTS is not handled by the Debian security team, but by a separate group of volunteers and companies interested in making it a success.  

And [Debian Extended LTS (ELTS)](https://deb.freexian.com/extended-lts) is its sister project, extending support to the Jessie release (+2 years after LTS support).

This was my twenty-seventh month as a Debian LTS and eighteenth month as a Debian ELTS paid contributor.  
I was assigned 58.25 hours for LTS and 60.00 hours for ELTS and worked on the following things:  
(I already worked for 20h in the last month (December) because of vacation :D)

#### LTS CVE Fixes and Announcements:

- Issued [DLA 2884-1](https://lists.debian.org/debian-lts-announce/2022/01/msg00019.html), fixing [CVE-2022-21661](https://security-tracker.debian.org/tracker/CVE-2022-21661), [CVE-2022-21662](https://security-tracker.debian.org/tracker/CVE-2022-21662), [CVE-2022-21663](https://security-tracker.debian.org/tracker/CVE-2022-21663), and [CVE-2022-21664](https://security-tracker.debian.org/tracker/CVE-2022-21664), for [wordpress](https://tracker.debian.org/pkg/wordpress).  
  For Debian 9 stretch, these problems have been fixed in version 4.7.22+dfsg-0+deb9u1.
- Issued [DLA 2885-1](https://lists.debian.org/debian-lts-announce/2022/01/msg00020.html), fixing [CVE-2021-3481](https://security-tracker.debian.org/tracker/CVE-2021-3481) and [CVE-2021-45930](https://security-tracker.debian.org/tracker/CVE-2021-45930), for [qtsvg-opensource-src](https://tracker.debian.org/pkg/qtsvg-opensource-src).  
  For Debian 9 stretch, these problems have been fixed in version 5.7.1~20161021-2.1+deb9u1.
- Issued [DLA 2895-1](https://lists.debian.org/debian-lts-announce/2022/01/msg00022.html), fixing [CVE-2021-3481](https://security-tracker.debian.org/tracker/CVE-2021-3481) and [CVE-2021-45930](https://security-tracker.debian.org/tracker/CVE-2021-45930), for [qt4-x11](https://tracker.debian.org/pkg/qt4-x11).  
  For Debian 9 stretch, these problems have been fixed in version 4:4.8.7+dfsg-11+deb9u3.
- Issued [DLA 2894-1](https://lists.debian.org/debian-lts-announce/2022/01/msg00024.html), fixing [CVE-2021-45417](https://security-tracker.debian.org/tracker/CVE-2021-45417), for [aide](https://tracker.debian.org/pkg/aide).  
  For Debian 9 stretch, these problems have been fixed in version 0.16-1+deb9u1.
- Issued [DSA 5067-1](https://lists.debian.org/debian-security-announce/2022/msg00034.html), fixing [CVE-2021-41816](https://security-tracker.debian.org/tracker/CVE-2021-41816), [CVE-2021-41817](https://security-tracker.debian.org/tracker/CVE-2021-41817), and [CVE-2021-41819](https://security-tracker.debian.org/tracker/CVE-2021-41819), for [ruby2.7](https://tracker.debian.org/pkg/ruby2.7).  
  For Debian 11 bullseye, these problems have been fixed in version 2.7.4-1+deb11u1.
- Also worked on the policykit-1 security update, rolled out by Salvatore.
- Simultaneously, I've been working on the samba and python* update.

#### ELTS CVE Fixes and Announcements:

- Issued [ELA 539-1](https://deb.freexian.com/extended-lts/updates/ela-539-1-wordpress/), fixing [CVE-2022-21661](https://security-tracker.debian.org/tracker/CVE-2022-21661), [CVE-2022-21662](https://security-tracker.debian.org/tracker/CVE-2022-21662), [CVE-2022-21663](https://security-tracker.debian.org/tracker/CVE-2022-21663), and [CVE-2022-21664](https://security-tracker.debian.org/tracker/CVE-2022-21664), for [wordpress](https://tracker.debian.org/pkg/wordpress).  
  For Debian 8 jessie, these problems have been fixed in version 4.1.34+dfsg-0+deb8u1.
- Issued [ELA 543-1](https://deb.freexian.com/extended-lts/updates/ela-543-1-qtsvg-opensource-src/), fixing [CVE-2018-19869](https://security-tracker.debian.org/tracker/CVE-2018-19869), [CVE-2021-3481](https://security-tracker.debian.org/tracker/CVE-2021-3481), and [CVE-2021-45930](https://security-tracker.debian.org/tracker/CVE-2021-45930), for [qtsvg-opensource-src](https://tracker.debian.org/pkg/qtsvg-opensource-src).  
  For Debian 8 jessie, these problems have been fixed in version 5.3.2-2+deb8u1.
- Issued [ELA 545-1](https://deb.freexian.com/extended-lts/updates/ela-545-1-aide/), fixing [CVE-2021-45417](https://security-tracker.debian.org/tracker/CVE-2021-45417), for [aide](https://tracker.debian.org/pkg/aide).  
  For Debian 8 jessie, these problems have been fixed in version 0.16~a2.git20130520-3+deb8u1.
- Issued [ELA 554-1](https://deb.freexian.com/extended-lts/updates/ela-554-1-qt4-x11/), fixing [CVE-2018-19872](https://security-tracker.debian.org/tracker/CVE-2018-19872), [CVE-2021-3481](https://security-tracker.debian.org/tracker/CVE-2021-3481), and [CVE-2021-45930](https://security-tracker.debian.org/tracker/CVE-2021-45930), for [qt4-x11](https://tracker.debian.org/pkg/qt4-x11).  
  For Debian 8 jessie, these problems have been fixed in version 4:4.8.6+git64-g5dc8b2b+dfsg-3+deb8u4.
- Issued [ELA 555-1](https://deb.freexian.com/extended-lts/updates/ela-555-1-shadow/), fixing [CVE-2017-12424](https://security-tracker.debian.org/tracker/CVE-2017-12424) and [CVE-2018-7169](https://security-tracker.debian.org/tracker/CVE-2018-7169), for [shadow](https://tracker.debian.org/pkg/shadow).  
  For Debian 8 jessie, these problems have been fixed in version 1:4.2-3+deb8u5.
- Issued [DSA 5066-1](https://lists.debian.org/debian-security-announce/2022/msg00033.html), fixing [CVE-2021-28965](https://security-tracker.debian.org/tracker/CVE-2021-28965), [CVE-2021-31799](https://security-tracker.debian.org/tracker/CVE-2021-31799), [CVE-2021-31810](https://security-tracker.debian.org/tracker/CVE-2021-31810), [CVE-2021-41817](https://security-tracker.debian.org/tracker/CVE-2021-41817), [CVE-2021-41819](https://security-tracker.debian.org/tracker/CVE-2021-41819), and [CVE-2021-32066](https://security-tracker.debian.org/tracker/CVE-2021-32066), for [ruby2.5](https://tracker.debian.org/pkg/ruby2.5).  
  For Debian 10 buster, these problems have been fixed in version 2.5.5-3+deb10u4.
- Worked on the policykit-1 ([ELA 551-1](https://deb.freexian.com/extended-lts/updates/ela-551-1-policykit-1/)) security update for jessie, fixing CVE-2021-4034, but was rolled out by Emilio due to a slight clash, but all good. :)  
- Been working on src:samba for CVE-2020-25717 to CVE-2020-25722 and CVE-2021-23192 for jessie and stretch, both.  
  The version difference b/w the suites are a bit too much for the patch(es) to be easily backported. Might need to unclaim, I think.
- Found the problem w/ libjdom1-java. Will have to roll the regression upload.  
- Also looking at python2.7 and python3.4 updates for jessie. Some regressions for the package has been reported on the Ubuntu side.  

#### Other (E)LTS Work:

- Front-desk duty from 24-01 to 30-01 for both LTS and ELTS.
- Triaged [wordpress](https://tracker.debian.org/pkg/wordpress),
[php-nette](https://tracker.debian.org/pkg/php-nette),
[samba](https://tracker.debian.org/pkg/samba),
[wordpress](https://tracker.debian.org/pkg/wordpress), and
[qtsvg-opensource-src](https://tracker.debian.org/pkg/qtsvg-opensource-src),
[qt4-x11](https://tracker.debian.org/pkg/qt4-x11),
[python2.7](https://tracker.debian.org/pkg/python2.7),
[python3.4](https://tracker.debian.org/pkg/python3.4),
[libspring-java](https://tracker.debian.org/pkg/libspring-java),
[librecad](https://tracker.debian.org/pkg/librecad),
[minetest](https://tracker.debian.org/pkg/minetest),
[spip](https://tracker.debian.org/pkg/spip),
[varnish](https://tracker.debian.org/pkg/varnish),
[libimage-exiftool-perl](https://tracker.debian.org/pkg/libimage-exiftool-perl),
[libsixel](https://tracker.debian.org/pkg/libsixel),
[openexr](https://tracker.debian.org/pkg/openexr),
[openssl](https://tracker.debian.org/pkg/openssl),
[phpmyadmin](https://tracker.debian.org/pkg/phpmyadmin),
[util-linux](https://tracker.debian.org/pkg/util-linux),
[shadow](https://tracker.debian.org/pkg/shadow),
[ruby2.5](https://tracker.debian.org/pkg/ruby2.5), and
[ruby2.7](https://tracker.debian.org/pkg/ruby2.7).
- Mark CVE-2022-21648/php-nette as not-affected for stretch and jessie.
- Mark CVE-2021-23803/php-nette as not-affected for stretch and jessie.
- Mark CVE-2021-22060/libspring-java as end-of-life for stretch.
- Mark CVE-2022-23935/libimage-exiftool-perl as no-dsa for stretch.
- Mark CVE-2021-45340/libsixel as no-dsa for stretch.
- Mark CVE-2021-45942/openexr as no-dsa for stretch.
- Mark CVE-2021-4160/openssl as no-dsa for stretch.
- Mark CVE-2022-23807/phpmyadmin as not-affected at all.
- Mark CVE-2022-23808/phpmyadmin as not-affected at all.
- Mark CVE-2022-23935/libimage-exiftool-perl as no-dsa for jessie.
- Mark CVE-2021-4160/openssl as no-dsa for jessie.
- Mark CVE-2021-3995/util-linux as not-affected for jessie.
- Mark CVE-2021-3996/util-linux as not-affected for jessie.
- Mark CVE-2022-23959/varnish as not-affected for jessie.
- Mark CVE-2021-4160/openssl as ignored instead for stretch.
- Auto EOL'ed 389-ds-base, mongodb, kfreebsd-10, spip, strongswan, libsixel, xen, connman, minetest, and linux for jessie.
- Attended monthly Debian LTS meeting.
- Answered questions (& discussions) on IRC (#debian-lts and #debian-elts).
- General and other discussions on LTS private and [public mailing list](https://lists.debian.org/debian-lts/2022/01/threads.html).

#### Debian LTS Survey

I've spent 5 hours on the LTS survey on the following bits:  
(however, I'll invoice them together next month)  
- Went through the content to put in the survey.
- Put some of them there according to the question type.
- Been going back and forth updating the status of the survey on the issue.

---

Until next time.  
`:wq` for today.
