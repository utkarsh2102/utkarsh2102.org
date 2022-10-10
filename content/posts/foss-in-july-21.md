+++
date = "2021-07-30 11:11:11 +0530"
title = "FOSS Activites in July 2021"
slug = "foss-in-july-21"
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

Here's my (twenty-second) monthly but brief update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 31st month of actively contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March 2019 and a [DD](https://wiki.debian.org/DebianDeveloper) on Christmas '19! \o/

I spent most of my free time on Clubhouse but still did everything I usually do (but did not go much beyond that, really).

Anyway, I did the following stuff in Debian:

#### Uploads and bug fixes:

- [libjdom1-java](https://tracker.debian.org/pkg/libjdom1-java) (1.1.3-2.1) - Fix for [CVE-2021-33813](https://security-tracker.debian.org/tracker/CVE-2021-33813)/[#990672](https://bugs.debian.org/990672).
- [rails](https://tracker.debian.org/pkg/rails) (2:6.0.3.7+dfsg-2) - Relax dependecny on ruby-marcel for Bullseye migration.
- [ruby2.7](https://tracker.debian.org/pkg/ruby2.7) (2.7.4-1) - Fix for {[CVE-2021-31799](https://security-tracker.debian.org/tracker/CVE-2021-31799), [CVE-2021-31810](https://security-tracker.debian.org/tracker/CVE-2021-31810), and [CVE-2021-32066](https://security-tracker.debian.org/tracker/CVE-2021-32066)}/[#990815](https://bugs.debian.org/990815).
- [libpam-tacplus](https://tracker.debian.org/pkg/libpam-tacplus) (1.3.8-2.1) - Fix for [CVE-2020-13881](https://security-tracker.debian.org/tracker/CVE-2020-13881)/[#962830](https://bugs.debian.org/962830) for Debian unstable, a.k.a. sid.
- [libpam-tacplus](https://tracker.debian.org/pkg/libpam-tacplus) (1.3.8-2+deb10u1) - Fix for [CVE-2020-13881](https://security-tracker.debian.org/tracker/CVE-2020-13881)/[#962830](https://bugs.debian.org/962830) for Debian 10, a.k.a. buster.
- [libjdom2-java](https://tracker.debian.org/pkg/libjdom2-java) (2.0.6-2.1) - Fix for [CVE-2021-33813](https://security-tracker.debian.org/tracker/CVE-2021-33813)/[#990671](https://bugs.debian.org/990671).

#### Other $things:

- Mentoring for newcomers.
- Moderation of -project mailing list.

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

This was my 6th month of actively contributing to [Ubuntu](https://ubuntu.com/about).
Now that I've joined [Canonical to work on Ubuntu full-time](https://utkarsh2102.com/posts/hello-canonical/), there's a bunch of things I do! \o/

I mostly worked on different things, I guess. But mostly on packaging [keylime](https://github.com/utkarsh2102/python-keylime) and some Google Agents upload(s) and SRU(s). Also did a lot of reviewing, et al.

I was too lazy to maintain a list of things I worked on so there's no concrete list atm. Maybe I'll get back to this section later or will start to list stuff from next month onward, as I've been doing before. :D

---

## Debian (E)LTS
{{< figure src="/images/debian-lts-small.png" >}}

[Debian Long Term Support (LTS)](https://www.freexian.com/en/services/debian-lts.html) is a project to extend the lifetime of all Debian stable releases to (at least) 5 years. Debian LTS is not handled by the Debian security team, but by a separate group of volunteers and companies interested in making it a success.  

And [Debian Extended LTS (ELTS)](https://deb.freexian.com/extended-lts) is its sister project, extending support to the Jessie release (+2 years after LTS support).

This was my twenty-second month as a Debian LTS and eleventh month as a Debian ELTS paid contributor.  
I was assigned 39.75 hours for LTS and 40.00 hours for ELTS and worked on the following things:  

#### LTS CVE Fixes and Announcements:

- Issued [DLA 2702-1](https://lists.debian.org/debian-lts-announce/2021/07/msg00002.html), fixing [CVE-2021-3630](https://security-tracker.debian.org/tracker/CVE-2021-3630), for [djvulibre](https://tracker.debian.org/pkg/djvulibre).  
  For Debian 9 stretch, these problems have been fixed in version 3.5.27.1-7+deb9u2.
- Issued [DLA 2703-1](https://lists.debian.org/debian-lts-announce/2021/07/msg00003.html), fixing [bug #908623](https://bugs.debian.org/908623) and [bug #932711](https://bugs.debian.org/932711), for [ieee-data](https://tracker.debian.org/pkg/ieee-data).  
  For Debian 9 stretch, these problems have been fixed in version 20160613.1+deb9u1.
- Issued [DLA 2718-1](https://lists.debian.org/debian-lts-announce/2021/07/msg00022.html), fixing [CVE-2020-24489](https://security-tracker.debian.org/tracker/CVE-2020-24489), [CVE-2020-24511](https://security-tracker.debian.org/tracker/CVE-2020-24511), [CVE-2020-24512](https://security-tracker.debian.org/tracker/CVE-2020-24512), and [CVE-2020-24513](https://security-tracker.debian.org/tracker/CVE-2020-24513), for [intel-microcode](https://tracker.debian.org/pkg/intel-microcode).  
  For Debian 9 stretch, these problems have been fixed in version 3.20210608.2~deb9u2.
- Issued [DLA 2730-1](https://lists.debian.org/debian-lts-announce/2021/08/msg00006.html), fixing [CVE-2020-13881](https://security-tracker.debian.org/tracker/CVE-2020-13881), for [libpam-tacplus](https://tracker.debian.org/pkg/libpam-tacplus).  
  For Debian 9 stretch, these problems have been fixed in version 1.3.8-2+deb9u1.
  - Also, uploaded [libpam-tacplus/1.3.8-2.1 to Debian unstable/sid](https://tracker.debian.org/news/1245344/accepted-libpam-tacplus-138-21-source-into-unstable/), fixing [CVE-2020-13881](https://security-tracker.debian.org/tracker/CVE-2020-13881)/[#962830](https://bugs.debian.org/962830).
  - Simultaneously, uploaded [libpam-tacplus/1.3.8-2+deb10u1 to Debian 10/buster](https://tracker.debian.org/news/1245501/accepted-libpam-tacplus-138-2deb10u1-source-amd64-into-proposed-updates-stable-new-proposed-updates/), fixing [CVE-2020-13881](https://security-tracker.debian.org/tracker/CVE-2020-13881)/[#962830](https://bugs.debian.org/962830.
- Issued [DLA 2731-1](https://lists.debian.org/debian-lts-announce/2021/08/msg00007.html), though CVEs aren't assigned yet, for [wordpress](https://tracker.debian.org/pkg/wordpress).  
  For Debian 9 stretch, these problems have been fixed in version 4.7.21+dfsg-0+deb9u1.

#### ELTS CVE Fixes and Announcements:

- Issued [ELA 465-1](https://deb.freexian.com/extended-lts/updates/ela-465-1-intel-microcode/), fixing [CVE-2020-24489](https://security-tracker.debian.org/tracker/CVE-2020-24489), [CVE-2020-24511](https://security-tracker.debian.org/tracker/CVE-2020-24511), [CVE-2020-24512](https://security-tracker.debian.org/tracker/CVE-2020-24512), and [CVE-2020-24513](https://security-tracker.debian.org/tracker/CVE-2020-24513), for [intel-microcode](https://tracker.debian.org/pkg/intel-microcode).  
  For Debian 8 jessie, these problems have been fixed in version 3.20210608.2~deb8u2.
- Issued [ELA 466-1](https://deb.freexian.com/extended-lts/updates/ela-466-1-libjdom1-java/), fixing [CVE-2021-33813](https://security-tracker.debian.org/tracker/CVE-2021-33813), for [libjdom1-java](https://tracker.debian.org/pkg/libjdom1-java).  
  For Debian 8 jessie, these problems have been fixed in version 1.1.3-1+deb8u1.
  - Also, uploaded [libjdom1-java/1.1.3-2.1 to Debian unstable/sid](https://tracker.debian.org/news/1245334/accepted-libjdom1-java-113-21-source-into-unstable/), fixing [CVE-2021-33813](https://security-tracker.debian.org/tracker/CVE-2021-33813)/[#990672](https://bugs.debian.org/990672).
  - Simultaneously, uploaded [libjdom2-java/2.0.6-2.1 to Debian unstable/sid](https://tracker.debian.org/news/1245371/accepted-libjdom2-java-206-21-source-into-unstable/) fixing [CVE-2021-33813](https://security-tracker.debian.org/tracker/CVE-2021-33813)/[#990672](https://bugs.debian.org/990672).
- Issued [ELA 467-1](https://deb.freexian.com/extended-lts/updates/ela-467-1-wordpress/), though CVEs aren't assigned yet, for [wordpress](https://tracker.debian.org/pkg/wordpress).
  For Debian 8 jessie, these problems have been fixed in version 4.1.33+dfsg-0+deb8u1.
- Issued [ELA 468-1](https://deb.freexian.com/extended-lts/updates/ela-468-1-libkohana2-php/), fixing [CVE-2016-10510](https://security-tracker.debian.org/tracker/CVE-2016-10510), for [libkohana2-php](https://tracker.debian.org/pkg/libkohana2-php).  
  For Debian 8 jessie, these problems have been fixed in version 2.3.4-2+deb8u1.
- Started working on src:usermode for fixing [bug #991808](https://bugs.debian.org/991808) but will probably fix src:libuser first, since it's also one of the supported packages.
- Started working on exiv2 issues but waiting for more CVEs to be alloted.

#### Other (E)LTS Work:

- Front-desk duty from 26-07 until 01-08 for both LTS and ELTS.
- Triaged [nodejs](https://tracker.debian.org/pkg/nodejs),
[mongodb](https://tracker.debian.org/pkg/mongodb),
[bluez](https://tracker.debian.org/pkg/bluez),
[libmatio](https://tracker.debian.org/pkg/libmatio),
[mbedtls](https://tracker.debian.org/pkg/mbedtls),
[node-url-parse](https://tracker.debian.org/pkg/node-url-parse),
[otrs2](https://tracker.debian.org/pkg/otrs2),
[polipo](https://tracker.debian.org/pkg/polipo),
[ruby-bindata](https://tracker.debian.org/pkg/ruby-bindata),
[util-linux](https://tracker.debian.org/pkg/util-linux),
[exiv2](https://tracker.debian.org/pkg/exiv2),
[ruby2.3](https://tracker.debian.org/pkg/ruby2.3),
[varnish](https://tracker.debian.org/pkg/varnish),
[gdal](https://tracker.debian.org/pkg/gdal),
[prosody](https://tracker.debian.org/pkg/prosody),
[glibc](https://tracker.debian.org/pkg/glibc),
[gdal](https://tracker.debian.org/pkg/gdal),
[rpm](https://tracker.debian.org/pkg/rpm),
[icu](https://tracker.debian.org/pkg/icu),
[ckeditor](https://tracker.debian.org/pkg/ckeditor),
[libvirt](https://tracker.debian.org/pkg/libvirt),
[libjdom1-java](https://tracker.debian.org/pkg/libjdom1-java),
[libjdom2-java](https://tracker.debian.org/pkg/libjdom2-java),
[tesseract](https://tracker.debian.org/pkg/tesseract),
[util-linux](https://tracker.debian.org/pkg/util-linux),
[qemu](https://tracker.debian.org/pkg/qemu),
[pillow](https://tracker.debian.org/pkg/pillow),
[tomcat8](https://tracker.debian.org/pkg/tomcat8),
[libcommons-compress-java](https://tracker.debian.org/pkg/libcommons-compress-java),
[389-ds-base](https://tracker.debian.org/pkg/389-ds-base), and
[intel-microcode](https://tracker.debian.org/pkg/intel-microcode).
- Mark CVE-2021-22930/nodejs as end-of-life for stretch.
- Mark CVE-2021-20333/mongodb as end-of-life for stretch.
- Mark CVE-2021-3652/389-ds-base as no-dsa for stretch.
- Mark CVE-2021-3658/bluez as no-dsa for stretch.
- Mark CVE-2020-19497/libmatio as no-dsa for stretch.
- Mark CVE-2021-24119/mbedtls as no-dsa for stretch.
- Mark CVE-2021-3664/node-url-parse as end-of-life for stretch.
- Mark CVE-2021-36091/otrs2 as no-dsa for stretch.
- Mark CVE-2021-36092/otrs2 as no-dsa for stretch.
- Mark CVE-2020-36420/polipo as ignored for stretch.
- Mark CVE-2021-32823/ruby-bindata as no-dsa for stretch.
- Mark CVE-2021-37600/util-linux as no-dsa for stretch.
- Mark CVE-2019-25050/gdal as not-affected for stretch.
- Mark CVE-2021-37601/prosody as not-affected for stretch instead.
- Mark CVE-2021-35942/glibc as no-dsa for jessie.
- Mark CVE-2021-36081/tesseract as not-affected for jessie.
- Mark CVE-2021-35939/rpm as no-dsa for jessie.
- Mark CVE-2021-35938/rpm as no-dsa for jessie.
- Mark CVE-2021-35937/rpm as no-dsa for jessie.
- Mark CVE-2021-30535/icu as not-affected for jessie.
- Mark CVE-2021-3667/libvirt as not-affected for jessie.
- Mark CVE-2021-3631/libvirt as no-dsa for jessie.
- Mark CVE-2021-21391/ckeditor as no-dsa for jessie.
- Mark CVE-2021-36090/libcommons-compress-java as no-dsa for jessie.
- Mark CVE-2021-3638/qemu as not-affected for jessie.
- Mark CVE-2021-34552/pillow as no-dsa for jessie.
- Mark CVE-2021-37600/util-linux as no-dsa for jessie.
- Mark CVE-2019-25050/gdal as not-affected for jessie.
- Mark CVE-2021-3658/bluez as no-dsa for jessie.
- Auto EOL'ed tiff, dcraw, libspring-security-2.0-java, rabbitmq-server, unrar-nonfree, darktable, mruby, htslib, ndpi, sam2p, libmatio, webkit2gtk, mongodb, otrs2, nodejs, vlc, jruby, asterisk, drupal7, libapache2-mod-auth-openidc, mosquitto, sylpheed, claws-mail, prosody, libapache2-mod-auth-mellon, and linux for jessie.
- Fix version of libjdom2-java's ELA.
- Attended monthly Debian LTS meeting.
- Answered questions (& discussions) on IRC (#debian-lts and #debian-elts).
- General and other discussions on LTS private and [public mailing list](https://lists.debian.org/debian-lts/2021/07/threads.html).

---

Until next time.  
`:wq` for today.
