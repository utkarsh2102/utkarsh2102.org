+++
date = "2021-06-01 00:00:00 +0530"
title = "FOSS Activites in May 2021"
slug = "foss-in-may-21"
images = [
    "/images/debian-logo-small.png",
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

Here's my (twentieth) monthly update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 29th month of actively contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March 2019 and a [DD](https://wiki.debian.org/DebianDeveloper) on Christmas '19! \o/

Interesting month, surprisingly. Lots of things happening and lots of moving parts; becoming the "new normal", I believe.
Anyhow, working on Ubuntu full-time has its own advantage and one of them is being able to work on Debian stuff! 🥰

So whilst I couldn't upload a lot of packages because of the freeze, here's what I worked on:

#### Uploads and bug fixes:

- [ruby-rack-cors](https://tracker.debian.org/pkg/ruby-rack-cors) (1.0.2-1+deb10u1) - Fix for [CVE-2019-18978](https://security-tracker.debian.org/tracker/CVE-2019-18978)/[#944849](https://bugs.debian.org/944849).
- [rails](https://tracker.debian.org/pkg/rails) (2:6.0.3.7+dfsg-1) - New upstream version, fixing {[CVE-2021-22904](https://security-tracker.debian.org/tracker/CVE-2021-22904), [CVE-2021-22902](https://security-tracker.debian.org/tracker/CVE-2021-22902), and [CVE-2021-22885](https://security-tracker.debian.org/tracker/CVE-2021-22885)}/[#988214](https://bugs.debian.org/988214).
- [ruby-marcel](https://tracker.debian.org/pkg/ruby-marcel) (1.0.1+dfsg-2) - Upload to unstable for rails.
- [python-aws-requests-auth](https://tracker.debian.org/pkg/python-aws-requests-auth) (0.4.3-2) - Enable build-time tests.
- [gist](https://tracker.debian.org/pkg/gist) (6.0.0-2) - Add patch to skip test when `$HTTP_PROXY` isn't set.
- [php-cache-lite](https://tracker.debian.org/pkg/php-cache-lite) (1.8.3-1) - New upstream version, fixing FTBFS w/ PHP 8.0.
- Sponsored upload of [htmldoc](https://tracker.debian.org/pkg/htmldoc) (1.9.3-1+deb10u1) to [buster-pu](https://tracker.debian.org/news/1241189/accepted-htmldoc-193-1deb10u1-source-all-amd64-into-proposed-updates-stable-new-proposed-updates/), fixing [CVE-2019-19630](https://security-tracker.debian.org/tracker/CVE-2019-19630) and [CVE-2021-20308](https://security-tracker.debian.org/tracker/CVE-2021-20308) for Håvard Flaget Aasen.
- Sponsored upload of [libbusiness-us-usps-webtools-perl](https://tracker.debian.org/pkg/libbusiness-us-usps-webtools-perl) (1.125-1) to [unstable](https://tracker.debian.org/news/1241495/accepted-libbusiness-us-usps-webtools-perl-1125-1-source-into-unstable/), fixing [#988330](https://bugs.debian.org/988330) for Yadd.
- Sponsored upload of [radsecproxy](https://tracker.debian.org/pkg/radsecproxy) (1.8.2-4) to [unstable](https://tracker.debian.org/news/1241891/accepted-radsecproxy-182-4-source-into-unstable/), fixing [CVE-2021-32642](https://security-tracker.debian.org/tracker/CVE-2021-32642) for Sven Hartge.

#### Other $things:

- Mentoring for newcomers and assisting people in BSP.
- Moderation of -project mailing list.

---

## Debian (E)LTS
{{< figure src="/images/debian-lts-small.png" >}}

[Debian Long Term Support (LTS)](https://www.freexian.com/en/services/debian-lts.html) is a project to extend the lifetime of all Debian stable releases to (at least) 5 years. Debian LTS is not handled by the Debian security team, but by a separate group of volunteers and companies interested in making it a success.  

And [Debian Extended LTS (ELTS)](https://deb.freexian.com/extended-lts) is its sister project, extending support to the Jessie release (+2 years after LTS support).

This was my twentieth month as a Debian LTS and eleventh month as a Debian ELTS paid contributor.  
I was assigned 29.75 hours for LTS and 40.00 hours for ELTS and worked on the following things:  

#### LTS CVE Fixes and Announcements:

- Issued [DLA 2654-1](https://lists.debian.org/debian-lts-announce/2021/05/msg00009.html), fixing [CVE-2021-29472](https://security-tracker.debian.org/tracker/CVE-2021-29472), for [composer](https://tracker.debian.org/pkg/composer).  
  For Debian 9 stretch, these problems have been fixed in version 1.2.2-1+deb9u1.
- Issued [DLA 2655-1](https://lists.debian.org/debian-lts-announce/2021/05/msg00010.html), fixing [CVE-2021-22885](https://security-tracker.debian.org/tracker/CVE-2021-22885) and [CVE-2021-22904](https://security-tracker.debian.org/tracker/CVE-2021-22904), for [rails](https://tracker.debian.org/pkg/rails).  
  For Debian 9 stretch, these problems have been fixed in version 2:4.2.7.1-1+deb9u5.
- Issued [DLA 2656-1](https://lists.debian.org/debian-lts-announce/2021/05/msg00011.html), fixing [CVE-2021-3504](https://security-tracker.debian.org/tracker/CVE-2021-3504), for [hivex](https://tracker.debian.org/pkg/hivex).  
  For Debian 9 stretch, these problems have been fixed in version 1.3.13-2+deb9u1.
- Issued [DLA 2659-1](https://lists.debian.org/debian-lts-announce/2021/05/msg00014.html), fixing [CVE-2018-10196](https://security-tracker.debian.org/tracker/CVE-2018-10196) and [CVE-2020-18032](https://security-tracker.debian.org/tracker/CVE-2020-18032), for [graphviz](https://tracker.debian.org/pkg/graphviz).  
  For Debian 9 stretch, these problems have been fixed in version 2.38.0-17+deb9u1.
- Issued [DLA 2662-1](https://lists.debian.org/debian-lts-announce/2021/05/msg00017.html), fixing [CVE-2021-32027](https://security-tracker.debian.org/tracker/CVE-2021-32027) and [CVE-2021-32028](https://security-tracker.debian.org/tracker/CVE-2021-32028), for [postgresql-9.6](https://tracker.debian.org/pkg/postgresql-9.6).  
  For Debian 9 stretch, these problems have been fixed in version 9.6.22-0+deb9u1. This update for done by the maintainer, Christoph Berg. I just took care of announcing and publishing the update.
- Uploaded [ruby-rack-cors](https://tracker.debian.org/news/1241341/accepted-ruby-rack-cors-102-1deb10u1-source-all-into-stable-embargoed-stable/) to buster-security, fixing [CVE-2019-18978](https://security-tracker.debian.org/tracker/CVE-2019-18978).
  For Debian 10 buster, these problems have been fixed in version 1.0.2-1+deb10u1.
- Issued [DLA 2663-1](https://lists.debian.org/debian-lts-announce/2021/05/msg00018.html), fixing [CVE-2021-22204](https://security-tracker.debian.org/tracker/CVE-2021-22204), for [libimage-exiftool-perl](https://tracker.debian.org/pkg/libimage-exiftool-perl).  
  For Debian 9 stretch, these problems have been fixed in version 10.40-1+deb9u1.

#### ELTS CVE Fixes and Announcements:

- Issued [ELA 425-1](https://deb.freexian.com/extended-lts/updates/ela-425-1-rails/), fixing [CVE-2021-22885](https://security-tracker.debian.org/tracker/CVE-2021-22885) and [CVE-2021-22904](https://security-tracker.debian.org/tracker/CVE-2021-22904), for [rails](https://tracker.debian.org/pkg/rails).  
  For Debian 8 jessie, these problems have been fixed in version 2:4.1.8-1+deb8u9.
- Uploaded [rails](https://tracker.debian.org/news/1241147/accepted-rails-26037dfsg-1-source-into-unstable/) to unstable, fixing [CVE-2021-22885](https://security-tracker.debian.org/tracker/CVE-2021-22885), [CVE-2021-22902](https://security-tracker.debian.org/tracker/CVE-2021-22902), and [CVE-2021-22904](https://security-tracker.debian.org/tracker/CVE-2021-22904).  
  For Debian sid, these problems have been fixed in version 2:6.0.3.7+dfsg-1.
- Issued [ELA 426-1](https://deb.freexian.com/extended-lts/updates/ela-426-1-hivex/), fixing [CVE-2021-3504](https://security-tracker.debian.org/tracker/CVE-2021-3504), for [hivex](https://tracker.debian.org/pkg/hivex).  
  For Debian 8 jessie, these problems have been fixed in version 1.3.10-2+deb8u3.
- Issued [ELA 428-1](https://deb.freexian.com/extended-lts/updates/ela-428-1-graphviz/), fixing [CVE-2018-10196](https://security-tracker.debian.org/tracker/CVE-2018-10196) and [CVE-2020-18032](https://security-tracker.debian.org/tracker/CVE-2020-18032), for [graphviz](https://tracker.debian.org/pkg/graphviz).  
  For Debian 8 jessie, these problems have been fixed in version 2.38.0-7+deb8u1.
- Issued [ELA 430-1](https://deb.freexian.com/extended-lts/updates/ela-430-1-libimage-exiftool-perl/), fixing [CVE-2021-22204](https://security-tracker.debian.org/tracker/CVE-2021-22204), for [libimage-exiftool-perl](https://tracker.debian.org/pkg/libimage-exiftool-perl).  
  For Debian 8 jessie, these problems have been fixed in version 9.74-1+deb8u1.

#### Other (E)LTS Work:

- Front-desk duty from 24-05 until 30-05 for both LTS and ELTS.
- Triaged [rails](https://tracker.debian.org/pkg/rails),
[libimage-exiftool-perl](https://tracker.debian.org/pkg/libimage-exiftool-perl),
[hivex](https://tracker.debian.org/pkg/hivex),
[graphviz](https://tracker.debian.org/pkg/graphviz),
[glibc](https://tracker.debian.org/pkg/glibc),
[libexosip2](https://tracker.debian.org/pkg/libexosip2),
[impacket](https://tracker.debian.org/pkg/impacket),
[node-ws](https://tracker.debian.org/pkg/node-ws),
[thunar](https://tracker.debian.org/pkg/thunar),
[libgrss](https://tracker.debian.org/pkg/libgrss),
[nginx](https://tracker.debian.org/pkg/nginx),
[postgresql-9.6](https://tracker.debian.org/pkg/postgresql-9.6),
[ffmpeg](https://tracker.debian.org/pkg/ffmpeg),
[composter](https://tracker.debian.org/pkg/composter), and
[curl](https://tracker.debian.org/pkg/curl).
- Mark CVE-2019-9904/graphviz as ignored for stretch and jessie.
- Mark CVE-2021-32029/postgresql-9.6 as not-affected for stretch.
- Mark CVE-2020-24020/ffmpeg as not-affected for stretch.
- Mark CVE-2020-22020/ffmpeg as postponed for stretch.
- Mark CVE-2020-22015/ffmpeg as ignored for stretch.
- Mark CVE-2020-21041/ffmpeg as postponed for stretch.
- Mark CVE-2021-33574/glibc as no-dsa for stretch & jessie.
- Mark CVE-2021-31800/impacket as no-dsa for stretch.
- Mark CVE-2021-32611/libexosip2 as no-dsa for stretch.
- Mark CVE-2016-20011/libgrss as ignored for stretch.
- Mark CVE-2021-32640/node-ws as no-dsa for stretch.
- Mark CVE-2021-32563/thunar as no-dsa for stretch.
- [LTS] Help test and review bind9 update for Emilio.
- [LTS] Suggest and add DEP8 tests for bind9 for stretch.
- [LTS] Sponsored upload of htmldoc to buster for Havard as a consequence of [#988289](https://bugs.debian.org/988289).
- [ELTS] Fix triage order for jetty and graphviz.
- [ELTS] Raise issue upstream about cloud-init; mock tests instead.
- [ELTS] Write to private ELTS list about triage ordering.
- [ELTS] Review Emilio's new script and write back feedback, mentioning extra file created, et al.
- [ELTS/LTS] Raise upgrade problems from LTS -> LTS+1 to the list. Thread [here](https://lists.debian.org/debian-lts/2021/05/msg00021.html).
  - Further help review and raise problems that could occur, et al.
- [LTS] Help explain path forward for firmware-nonfree update to Ola. Thread [here](https://lists.debian.org/debian-lts/2021/05/msg00030.html).
- [ELTS] Revert entries of TEMP-0000000-16B7E7 and TEMP-0000000-1C4729; CVEs assigned & fix ELTS tracker build.
- Auto EOL'ed linux, libgrss, node-ws, and inspircd for jessie.
- Attended monthly Debian LTS meeting, which didn't happen, heh.
- Answered questions (& discussions) on IRC (#debian-lts and #debian-elts).
- General and other discussions on LTS private and [public mailing list](https://lists.debian.org/debian-lts/2021/05/threads.html).

---

Until next time.  
`:wq` for today.
