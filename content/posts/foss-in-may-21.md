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

This was my nineteenth month as a Debian LTS and tenth month as a Debian ELTS paid contributor.  
I was assigned 60.00 hours for LTS and 60.00 hours for ELTS and worked on the following things:  

#### LTS CVE Fixes and Announcements:

#### ELTS CVE Fixes and Announcements:

#### Other (E)LTS Work:

- Private ELTS-related discussion on the ELTS list (+ w/ Raphael).
- Auto EOL'ed webkit2gtk, python-bleach, tika, linux, ircii, spice-vdagent, libspring-security-2.0-java, file-roller, rustc, python-django-registration, gsoap, thunderbird, mosquitto, ruby-sidekiq, gnuchess, libpodofo, unbound, drupal7, 389-ds-base, and scrollz for jessie.
- Answered questions (& discussions) on IRC (#debian-lts and #debian-elts).
- General and other discussions on LTS private and [public mailing list](https://lists.debian.org/debian-lts/2021/02/threads.html).

---

Until next time.  
`:wq` for today.
