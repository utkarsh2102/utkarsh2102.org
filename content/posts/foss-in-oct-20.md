+++
date = "2020-11-01 11:30:00 +0530"
title = "FOSS Activites in October 2020"
slug = "foss-in-oct-20"
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

Here's my (thirteenth) monthly update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 22nd month of contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March last year and a [DD](https://wiki.debian.org/DebianDeveloper) last Christmas! \o/

Whilst busy with my undergrad, I could still make some time out for contributing to Debian (I always do!).
Here are the following things I did in Debian this month:

#### Uploads and bug fixes:

- [ruby-mini-magick](https://tracker.debian.org/pkg/ruby-mini-magick) (4.10.1-1) - Fixing FTBFS, [bug #966936](https://bugs.debian.org/966936).
- [ruby2.7](https://tracker.debian.org/pkg/ruby2.7) (2.7.1-4) - Fixing [CVE-2020-25613](https://security-tracker.debian.org/tracker/CVE-2020-25613).
- [net-tools](https://tracker.debian.org/pkg/net-tools) (1.60+git20181103.0eebece-1) - Fixing bug [#812886](https://bugs.debian.org/812886), [#653117](https://bugs.debian.org/653117), [#621752](https://bugs.debian.org/621752), and [#549397](https://bugs.debian.org/549397).
- [libgit2](https://tracker.debian.org/pkg/libgit2) (1.0.1+dfsg.1-1) - New upstream version, v1.0.1.
- [rails](https://tracker.debian.org/pkg/rails) (2:6.0.3.4+dfsg-1) - Fixing [CVE-2020-8264](https://security-tracker.debian.org/tracker/CVE-2020-8264)/[bug #971988](https://bugs.debian.org/971988).
- [ruby2.7](https://tracker.debian.org/pkg/ruby2.7) (2.7.2-1) - New upstream version, v2.7.2.
- [bundler](https://tracker.debian.org/pkg/bundler) (2.1.4-3) - Fixing [bug #962463](https://bugs.debian.org/962463).
- [ruby2.5](https://tracker.debian.org/pkg/ruby2.5) (2.5.5-3+deb10u3) - Fixing [CVE-2020-25613](https://security-tracker.debian.org/tracker/CVE-2020-25613).
- [ruby2.7](https://tracker.debian.org/pkg/ruby2.7) (2.7.2-2) - Fixing bug [#970469](https://bugs.debian.org/970469), [#969130](https://bugs.debian.org/969130), and [#968203](https://bugs.debian.org/968203).
- [ruby3.0](https://tracker.debian.org/pkg/ruby3.0) (3.0.0~preview1-1) - Introducing ruby3.0, FTW!
- [ruby-mysql2](https://tracker.debian.org/pkg/ruby-mysql2) (0.5.3-1) - Fixing FTBFS, [bug #923727](https://bugs.debian.org/923727).
- [ruby-rubocop-packaging](https://tracker.debian.org/pkg/ruby-rubocop-packaging) (0.5.1-1) - Make it compatible with RuboCop v1.0.

#### Other $things:

- Attended the Debian Ruby team meeting. Logs [here](http://meetbot.debian.net/debian-ruby/2020/debian-ruby.2020-10-02-16.37.html).
- Mentoring for newcomers.
- FTP Trainee reviewing.
- Moderation of -project mailing list.
- Sponsored `phpmyadmin`, `php-bacon-baconqrcode`, `twig`, `php-dasprid-enum`, `sql-parser`, and `mariadb-mysql-kbs` for William.

---

## Debian (E)LTS

This was my thirteenth month as a Debian LTS and fourth month as a Debian ELTS paid contributor.  
I was assigned 20.75 hours for LTS and 30.00 hours for ELTS and worked on the following things:  

#### Other (E)LTS Work:

- Front-desk duty from 28-09 to 04-10 and from 26-10 until 01-10 for both LTS and ELTS.
- Triaged [libproxy](https://tracker.debian.org/pkg/libproxy),
[libvirt](https://tracker.debian.org/pkg/libvirt),
[libonig](https://tracker.debian.org/pkg/libonig),
[ant](https://tracker.debian.org/pkg/ant),
[erlang](https://tracker.debian.org/pkg/erlang),
[ruby2.3](https://tracker.debian.org/pkg/ruby2.3),
[jruby](https://tracker.debian.org/pkg/jruby),
[dpdk](https://tracker.debian.org/pkg/dpdk),
[php7.0](https://tracker.debian.org/pkg/php7.0),
[spice](https://tracker.debian.org/pkg/spice),
[spice-gtk](https://tracker.debian.org/pkg/spice-gtk),
[wireshark](https://tracker.debian.org/pkg/wireshark),
[djangorestframework](https://tracker.debian.org/pkg/djangorestframework),
[python-urllib3](https://tracker.debian.org/pkg/python-urllib3),
[python-cryptography](https://tracker.debian.org/pkg/python-cryptography),
[qtsvg-opensource-src](https://tracker.debian.org/pkg/qtsvg-opensource-src), and
[open-build-service](https://tracker.debian.org/pkg/open-build-service).
- Marked CVE-2020-26137/python-urllib3 as no-dsa for Stretch and Jessie.
- Marked CVE-2020-1437{4,5,6,7,8}/dpdk as no-dsa for Stretch.
- Marked CVE-2020-2586{2,3}/wireshark as postponed for Stretch.
- Marked CVE-2020-25626/djangorestframework as no-dsa for Stretch.
- Marked CVE-2020-11979/ant as not-affected for Jessie.
- Marked CVE-2020-25623/erlang as not-affected for Jessie.
- Marked CVE-2020-25659/python-cryptography as no-dsa for Stretch and Jessie.
- Auto EOL'ed jruby, libjs-handlebars, linux, pluxml, mupdf, and djangorestframework for Jessie.
- [E/LTS] Worked on putting survey online, deployed [LTS Team Pages](https://lts-team.pages.debian.net/) \o/
- [ELTS] Fix suite-name in ela-needed file and fix other tags and ordering of triages to fix erros in the security tracker.
- [LTS] Sent out invitations for the meeting.
- Attended the sixth private LTS meeting.
- General discussion on LTS private and [public mailing list](https://lists.debian.org/debian-lts/2020/10/threads.html).

#### LTS CVE Fixes and Announcements:

- Issued [DLA 2389-1](https://lists.debian.org/debian-lts-announce/2020/10/msg00000.html), fixing [CVE-2019-18978](https://security-tracker.debian.org/tracker/CVE-2019-18978), for [ruby-rack-cors](https://tracker.debian.org/pkg/ruby-rack-cors).  
  For Debian 9 Stretch, these problems have been fixed in version 0.4.0-1+deb9u2.
- Issued [DLA 2390-1](https://lists.debian.org/debian-lts-announce/2020/10/msg00001.html), fixing [CVE-2019-18848](https://security-tracker.debian.org/tracker/CVE-2019-18848), for [ruby-json-jwt](https://tracker.debian.org/pkg/ruby-json-jwt).  
  For Debian 9 Stretch, these problems have been fixed in version 1.6.2-1+deb9u2.
- Issued [DLA 2391-1](https://lists.debian.org/debian-lts-announce/2020/10/msg00002.html), fixing [CVE-2020-25613](https://security-tracker.debian.org/tracker/CVE-2020-25613), for [ruby2.3](https://tracker.debian.org/pkg/ruby2.3).  
  For Debian 9 Stretch, these problems have been fixed in version 2.3.3-1+deb9u9.
- Issued [DLA 2392-1](https://lists.debian.org/debian-lts-announce/2020/10/msg00003.html), fixing [CVE-2020-25613](https://security-tracker.debian.org/tracker/CVE-2020-25613), for [jruby](https://tracker.debian.org/pkg/jruby).  
  For Debian 9 Stretch, these problems have been fixed in version 1.7.26-1+deb9u3.
- Uploaded ruby2.5 to buster, fixing CVE-2020-25613.
  For Debian 10 Buster, these problems have been fixed in version 2.5.5-3+deb10u3.
- Uploaded ruby2.7 to unstable, fixing CVE-2020-25613.
  For Debian Sid, these problems have been fixed in version 2.7.1-4.
- Uploaded rails to unstable, fixing CVE-2020-8264.
  For Debian Sid, these problems have been fixed in version 2:6.0.3.4+dfsg-1.

#### ELTS CVE Fixes and Announcements:

- Issued [ELA 290-1](https://deb.freexian.com/extended-lts/updates/ela-290-1-ruby2.1/), fixing [CVE-2020-25613](https://security-tracker.debian.org/tracker/CVE-2020-25613), for [ruby2.1](https://tracker.debian.org/pkg/ruby2.1).  
  For Debian 8 Jessie, these problems have been fixed in version 2.1.5-2+deb8u11.
- Issued [ELA 292-1](https://deb.freexian.com/extended-lts/updates/ela-292-1-libonig/), fixing [CVE-2020-26159](https://security-tracker.debian.org/tracker/CVE-2020-26159), for [libonig](https://tracker.debian.org/pkg/libonig).  
  For Debian 8 Jessie, these problems have been fixed in version 5.9.5-3.2+deb8u5.
- Issued [ELA 297-1](https://deb.freexian.com/extended-lts/updates/ela-297-1-packagekit/), fixing [CVE-2020-16121](https://security-tracker.debian.org/tracker/CVE-2020-16121) and [CVE-2020-16122](https://security-tracker.debian.org/tracker/CVE-2020-16122), for [packagekit](https://tracker.debian.org/pkg/packagekit).  
  For Debian 8 Jessie, these problems have been fixed in version 1.0.1-2+deb8u1.
- Issued [ELA 298-1](https://deb.freexian.com/extended-lts/updates/ela-298-1-spice/), fixing [CVE-2020-14355](https://security-tracker.debian.org/tracker/CVE-2020-14355), for [spice](https://tracker.debian.org/pkg/spice).  
  For Debian 8 Jessie, these problems have been fixed in version 0.12.5-1+deb8u8.
- Issued [ELA 299-1](https://deb.freexian.com/extended-lts/updates/ela-299-1-spice-gtk/), fixing [CVE-2020-14355](https://security-tracker.debian.org/tracker/CVE-2020-14355), for [spice-gtk](https://tracker.debian.org/pkg/spice-gtk).  
  For Debian 8 Jessie, these problems have been fixed in version 0.25-1+deb8u2.
- Started working on openldap vulnerabilities, CVEs are yet to be assigned.

---

Until next time.  
`:wq` for today.
