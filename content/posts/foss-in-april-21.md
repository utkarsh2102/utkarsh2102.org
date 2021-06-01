+++
date = "2021-05-01 19:00:00 +0530"
title = "FOSS Activites in April 2021"
slug = "foss-in-april-21"
images = [
    "/images/debian-logo-small.png",
    "/images/debian-lts-small.png",
    "/images/salzburg_bsp.png",
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

Here's my (nineteenth) monthly update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 28th month of actively contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March 2019 and a [DD](https://wiki.debian.org/DebianDeveloper) on Christmas '19! \o/

Crazy month, as always. Lots of things happening and lots of moving parts.  
Now that I am working on Ubuntu full-time, I barely get much time to do any extra stuff. Then the massive COVID wave that has plunged India had made this month further crazier. More on that later, maybe. IDK.

Anyway, I did some Debian stuff, thanks to Salzburg BSP (more down below). I worked on the following stuff:

#### Uploads and bug fixes:

- [ruby2.7](https://tracker.debian.org/pkg/ruby2.7) (2.7.3-1) - New upstream version, fixing [CVE-2021-28965](https://security-tracker.debian.org/tracker/CVE-2021-28965)/[#986807](https://bugs.debian.org/986807).
- [jackson-databind](https://tracker.debian.org/pkg/jackson-databind) (2.9.8-3+deb10u3) - buster-pu upload, fixing [CVE-2020-24616](https://security-tracker.debian.org/tracker/CVE-2020-24616), [CVE-2020-24750](https://security-tracker.debian.org/tracker/CVE-2020-24750), [CVE-2020-25649](https://security-tracker.debian.org/tracker/CVE-2020-25649), [CVE-2020-35490](https://security-tracker.debian.org/tracker/CVE-2020-35490), [CVE-2020-35491](https://security-tracker.debian.org/tracker/CVE-2020-35491), [CVE-2020-35728](https://security-tracker.debian.org/tracker/CVE-2020-35728), [CVE-2020-36179](https://security-tracker.debian.org/tracker/CVE-2020-36179), [CVE-2020-36180](https://security-tracker.debian.org/tracker/CVE-2020-36180), [CVE-2020-36181](https://security-tracker.debian.org/tracker/CVE-2020-36181), [CVE-2020-36182](https://security-tracker.debian.org/tracker/CVE-2020-36182), [CVE-2020-36183](https://security-tracker.debian.org/tracker/CVE-2020-36183), [CVE-2020-36184](https://security-tracker.debian.org/tracker/CVE-2020-36184), [CVE-2020-36185](https://security-tracker.debian.org/tracker/CVE-2020-36185), [CVE-2020-36186](https://security-tracker.debian.org/tracker/CVE-2020-36186), [CVE-2020-36187](https://security-tracker.debian.org/tracker/CVE-2020-36187), [CVE-2020-36188](https://security-tracker.debian.org/tracker/CVE-2020-36188), [CVE-2020-36189](https://security-tracker.debian.org/tracker/CVE-2020-36189), and [CVE-2021-20190](https://security-tracker.debian.org/tracker/CVE-2021-20190).
- [ruby-librarian](https://tracker.debian.org/pkg/ruby-librarian) (0.6.4-3) - Fixing autpkgtest; cf: [#987113](https://bugs.debian.org/987113).
- [opendmarc](https://tracker.debian.org/pkg/opendmarc) (1.3.2-6+deb10u2) - buster-pu upload, fixing [CVE-2020-12460](https://security-tracker.debian.org/tracker/CVE-2020-12460)/[#966464](https://bugs.debian.org/966464).
- Sponsored upload of [fluidsynth](https://tracker.debian.org/pkg/fluidsynth) (2.1.7-1.1) to [unstable](https://tracker.debian.org/news/1239551/accepted-fluidsynth-217-11-source-into-unstable/), fixing [CVE-2021-28421](https://security-tracker.debian.org/tracker/CVE-2021-28421)/[#987168](https://bugs.debian.org/987168) for Reiner Herrmann.
- Sponsored upload of [fluidsynth](https://tracker.debian.org/pkg/fluidsynth) (1.1.11-1+deb10u1) to [buster](https://tracker.debian.org/news/1240246/accepted-fluidsynth-1111-1deb10u1-source-amd64-into-proposed-updates-stable-new-proposed-updates/), fixing [CVE-2021-28421](https://security-tracker.debian.org/tracker/CVE-2021-28421)/[#987168](https://bugs.debian.org/987168) for Reiner Herrmann.
- Sponsored upload of [libpam-alreadyloggedin](https://tracker.debian.org/pkg/libpam-alreadyloggedin) (0.3-9) to [unstable](https://tracker.debian.org/news/1239618/accepted-libpam-alreadyloggedin-03-9-source-into-unstable/), fixing [#958224](https://bugs.debian.org/958224), [#986247](https://bugs.debian.org/986247), and [#969122](https://bugs.debian.org/969122) for Reiner Herrmann.

#### Other $things:

- Mentoring for newcomers and assisting people in BSP.
- Moderation of -project mailing list.

---

## Salzburg BSP 2021

This was my first virtual BSP and the first BSP in Salzburg and it was absolutely amazing!  
Many kudos to Bernd Zeimetz for organizing it so smoothly and wonderfully, for real! \o/

We had a bunch of amazing sessions, besides hacking, of course, like:
- yoga,
- sports,
- games, and
- datacenter tour -> which was super!

We also had lots of things happening at #debian-bsp-2021-szg and did a lot of work.  
Whilst everything we did is available on the [pad](https://pad.riseup.net/p/bsp-2021-04-AT-Salzburg), I work on the following things:
- [deki/utkarsh]: CVE-2021-28421/fluidsynth (sid); cf: #987168/#987471.
- [deki/utkarsh]: CVE-2021-28421/fluidsynth (buster); cf: #987168/#987494.
- [utkarsh]: 18 CVEs for jackson-databind (buster); cf: #987489.
- [utkarsh]: fix for ruby-librarian/#987113 (unblock request: #987501).
- [utkarsh]: 17 CVEs for jackson-databind (stretch); LTS upload.
- [utkarsh]: CVE-2020-12460/opendmarc (stretch); LTS upload.
- [utkarsh]: CVE-2020-12460/opendmarc (buster); cf: #987531.
- [deki/utkarsh]: libpam-alreadyloggedin, broken autopkgtest; #958224
- [deki/utkarsh]: libpam-alreadyloggedin, installed in wrong directory; #986247
- [deki/utkarsh]: libpam-alreadyloggedin, FTCBFS; #969122
- [donfede/utkarsh] 10 CVEs for salt (buster)
- [donfede/utkarsh] 10 CVEs for salt (bullseye)

And finally, we clicked a picture! \o/
![](/images/salzburg_bsp.png#center)

---

## Debian (E)LTS
{{< figure src="/images/debian-lts-small.png" >}}

[Debian Long Term Support (LTS)](https://www.freexian.com/en/services/debian-lts.html) is a project to extend the lifetime of all Debian stable releases to (at least) 5 years. Debian LTS is not handled by the Debian security team, but by a separate group of volunteers and companies interested in making it a success.  

And [Debian Extended LTS (ELTS)](https://deb.freexian.com/extended-lts) is its sister project, extending support to the Jessie release (+2 years after LTS support).

This was my nineteenth month as a Debian LTS and tenth month as a Debian ELTS paid contributor.  
I was assigned 60.00 hours for LTS and 60.00 hours for ELTS and worked on the following things:  

#### LTS CVE Fixes and Announcements:

- Issued [DLA 2615-1](https://lists.debian.org/debian-lts-announce/2021/04/msg00000.html), fixing [CVE-2020-1946](https://security-tracker.debian.org/tracker/CVE-2020-1946), for [spamassassin](https://tracker.debian.org/pkg/spamassassin).  
  For Debian 9 stretch, these problems have been fixed in version 3.4.2-1~deb9u4.
- Issued [DLA 2624-1](https://lists.debian.org/debian-lts-announce/2021/04/msg00010.html), fixing [CVE-2021-20307](https://security-tracker.debian.org/tracker/CVE-2021-20307), for [libpano13](https://tracker.debian.org/pkg/libpano13).  
  For Debian 9 stretch, these problems have been fixed in version 2.9.19+dfsg-2+deb9u1.
- Issued [DLA 2625-1](https://lists.debian.org/debian-lts-announce/2021/04/msg00011.html), fixing [CVE-2021-28374](https://security-tracker.debian.org/tracker/CVE-2021-28374), for [courier-authlib](https://tracker.debian.org/pkg/courier-authlib).  
  For Debian 9 stretch, these problems have been fixed in version 0.66.4-9+deb9u1.
- Issued [DLA 2626-1](https://lists.debian.org/debian-lts-announce/2021/04/msg00012.html), fixing [CVE-2021-1405](https://security-tracker.debian.org/tracker/CVE-2021-1405), for [clamav](https://tracker.debian.org/pkg/clamav).  
  For Debian 9 stretch, these problems have been fixed in version 0.102.4+dfsg-0+deb9u2.
- Uploaded [ruby2.7](https://tracker.debian.org/news/1239104/accepted-ruby27-273-1-source-into-unstable/) to [sid](https://bugs.debian.org/986807), fixing [CVE-2021-28965](https://security-tracker.debian.org/tracker/CVE-2021-28965).  
  For Debian sid, these problems have been fixed in version 2.7.3-1.
- Issued [DLA 2630-1](https://lists.debian.org/debian-lts-announce/2021/04/msg00017.html), fixing [CVE-2021-29447](https://security-tracker.debian.org/tracker/CVE-2021-29447) and [CVE-2021-29450](https://security-tracker.debian.org/tracker/CVE-2021-29450), for [wordpress](https://tracker.debian.org/pkg/wordpress).  
  For Debian 9 stretch, these problems have been fixed in version 4.7.20+dfsg-1+deb9u1.
- Issued [DLA 2633-1](https://lists.debian.org/debian-lts-announce/2021/04/msg00020.html), fixing [CVE-2021-23961](https://security-tracker.debian.org/tracker/CVE-2021-23961), [CVE-2021-23994](https://security-tracker.debian.org/tracker/CVE-2021-23994), [CVE-2021-23995](https://security-tracker.debian.org/tracker/CVE-2021-23995), [CVE-2021-23998](https://security-tracker.debian.org/tracker/CVE-2021-23998), [CVE-2021-23999](https://security-tracker.debian.org/tracker/CVE-2021-23999), [CVE-2021-24002](https://security-tracker.debian.org/tracker/CVE-2021-24002), [CVE-2021-29945](https://security-tracker.debian.org/tracker/CVE-2021-29945), and [CVE-2021-29946](https://security-tracker.debian.org/tracker/CVE-2021-29946), for [firefox-esr](https://tracker.debian.org/pkg/firefox-esr).  
  For Debian 9 stretch, these problems have been fixed in version 78.10.0esr-1~deb9u1. Thanks, Emilio, for all your help on this! \o/
- Issued [DLA 2638-1](https://lists.debian.org/debian-lts-announce/2021/04/msg00025.html), fixing [CVE-2020-24616](https://security-tracker.debian.org/tracker/CVE-2020-24616), [CVE-2020-24750](https://security-tracker.debian.org/tracker/CVE-2020-24750), [CVE-2020-35490](https://security-tracker.debian.org/tracker/CVE-2020-35490), [CVE-2020-35491](https://security-tracker.debian.org/tracker/CVE-2020-35491), [CVE-2020-35728](https://security-tracker.debian.org/tracker/CVE-2020-35728), [CVE-2020-36179](https://security-tracker.debian.org/tracker/CVE-2020-36179), [CVE-2020-36180](https://security-tracker.debian.org/tracker/CVE-2020-36180), [CVE-2020-36181](https://security-tracker.debian.org/tracker/CVE-2020-36181), [CVE-2020-36182](https://security-tracker.debian.org/tracker/CVE-2020-36182), [CVE-2020-36183](https://security-tracker.debian.org/tracker/CVE-2020-36183), [CVE-2020-36184](https://security-tracker.debian.org/tracker/CVE-2020-36184), [CVE-2020-36185](https://security-tracker.debian.org/tracker/CVE-2020-36185), [CVE-2020-36186](https://security-tracker.debian.org/tracker/CVE-2020-36186), [CVE-2020-36187](https://security-tracker.debian.org/tracker/CVE-2020-36187), [CVE-2020-36188](https://security-tracker.debian.org/tracker/CVE-2020-36188), [CVE-2020-36189](https://security-tracker.debian.org/tracker/CVE-2020-36189), [CVE-2021-20190](https://security-tracker.debian.org/tracker/CVE-2021-20190), and [CVE-2020-25649](https://security-tracker.debian.org/tracker/CVE-2020-25649), for [jackson-databind](https://tracker.debian.org/pkg/jackson-databind).  
  For Debian 9 stretch, these problems have been fixed in version 2.8.6-1+deb9u9.
- Issued [DLA 2639-1](https://lists.debian.org/debian-lts-announce/2021/04/msg00026.html), fixing [CVE-2020-12460](https://security-tracker.debian.org/tracker/CVE-2020-12460), for [opendmarc](https://tracker.debian.org/pkg/opendmarc).  
  For Debian 9 stretch, these problems have been fixed in version 1.3.2-2+deb9u3.
- Uploaded [fluidsynth](https://tracker.debian.org/news/1239551/accepted-fluidsynth-217-11-source-into-unstable/) to [sid](https://bugs.debian.org/987168), fixing [CVE-2021-28421](https://security-tracker.debian.org/tracker/CVE-2021-28421).  
  For Debian sid, these problems have been fixed in version 2.1.7-1.1. Thanks to Reiner Herrmann for their work.
- Uploaded [fluidsynth](https://tracker.debian.org/pkg/fluidsynth) to [buster-pu](https://bugs.debian.org/987494), fixing [CVE-2021-28421](https://security-tracker.debian.org/tracker/CVE-2021-28421).  
  For Debian sid, these problems have been fixed in version 2.1.7-1.1. Thanks to Reiner Herrmann for their work.

#### ELTS CVE Fixes and Announcements:

- Issued [ELA 396-1](https://deb.freexian.com/extended-lts/updates/ela-396-1-underscore/), fixing [CVE-2021-23358](https://security-tracker.debian.org/tracker/CVE-2021-23358), for [underscore](https://tracker.debian.org/pkg/underscore).  
  For Debian 8 jessie, these problems have been fixed in version 1.7.0~dfsg-1+deb8u1.
- Issued [ELA 397-1](https://deb.freexian.com/extended-lts/updates/ela-397-1-spamassassin/), fixing [CVE-2020-1946](https://security-tracker.debian.org/tracker/CVE-2020-1946), for [spamassassin](https://tracker.debian.org/pkg/spamassassin).  
  For Debian 8 jessie, these problems have been fixed in version 3.4.2-0+deb8u4.
- Issued [ELA 400-1](https://deb.freexian.com/extended-lts/updates/ela-400-1-wordpress/), fixing [CVE-2020-25286](https://security-tracker.debian.org/tracker/CVE-2020-25286), [CVE-2020-28032](https://security-tracker.debian.org/tracker/CVE-2020-28032), [CVE-2020-28033](https://security-tracker.debian.org/tracker/CVE-2020-28033), [CVE-2020-28034](https://security-tracker.debian.org/tracker/CVE-2020-28034), [CVE-2020-28035](https://security-tracker.debian.org/tracker/CVE-2020-28035), [CVE-2020-28036](https://security-tracker.debian.org/tracker/CVE-2020-28036), [CVE-2020-28037](https://security-tracker.debian.org/tracker/CVE-2020-28037), [CVE-2020-28038](https://security-tracker.debian.org/tracker/CVE-2020-28038), [CVE-2020-28039](https://security-tracker.debian.org/tracker/CVE-2020-28039), and [CVE-2020-28040](https://security-tracker.debian.org/tracker/CVE-2020-28040), for [wordpress](https://tracker.debian.org/pkg/wordpress).  
  For Debian 8 jessie, these problems have been fixed in version 4.1.32+dfsg-0+deb8u1.
- Help issued [ELA 401-1](https://deb.freexian.com/extended-lts/updates/ela-401-1-tomcat7/), fixing [CVE-2021-25329](https://security-tracker.debian.org/tracker/CVE-2021-25329) and [CVE-2020-9484](https://security-tracker.debian.org/tracker/CVE-2020-9484), for [tomcat7](https://tracker.debian.org/pkg/tomcat7), along with Markus.  
  For Debian 8 jessie, these problems have been fixed in version 7.0.56-3+really7.0.100-1+deb8u3.
- Issued [ELA 403-1](https://deb.freexian.com/extended-lts/updates/ela-403-1-jackson-databind/), fixing [CVE-2020-24616](https://security-tracker.debian.org/tracker/CVE-2020-24616), [CVE-2020-24750](https://security-tracker.debian.org/tracker/CVE-2020-24750), [CVE-2020-25649](https://security-tracker.debian.org/tracker/CVE-2020-25649), [CVE-2020-35490](https://security-tracker.debian.org/tracker/CVE-2020-35490), [CVE-2020-35491](https://security-tracker.debian.org/tracker/CVE-2020-35491), [CVE-2020-35728](https://security-tracker.debian.org/tracker/CVE-2020-35728), [CVE-2020-36179](https://security-tracker.debian.org/tracker/CVE-2020-36179), [CVE-2020-36180](https://security-tracker.debian.org/tracker/CVE-2020-36180), [CVE-2020-36181](https://security-tracker.debian.org/tracker/CVE-2020-36181), [CVE-2020-36182](https://security-tracker.debian.org/tracker/CVE-2020-36182), [CVE-2020-36183](https://security-tracker.debian.org/tracker/CVE-2020-36183), [CVE-2020-36184](https://security-tracker.debian.org/tracker/CVE-2020-36184), [CVE-2020-36185](https://security-tracker.debian.org/tracker/CVE-2020-36185), [CVE-2020-36186](https://security-tracker.debian.org/tracker/CVE-2020-36186), [CVE-2020-36187](https://security-tracker.debian.org/tracker/CVE-2020-36187), [CVE-2020-36188](https://security-tracker.debian.org/tracker/CVE-2020-36188), [CVE-2020-36189](https://security-tracker.debian.org/tracker/CVE-2020-36189), and [CVE-2021-20190](https://security-tracker.debian.org/tracker/CVE-2021-20190), for [jackson-databind](https://tracker.debian.org/pkg/jackson-databind).  
  For Debian 8 jessie, these problems have been fixed in version 2.4.2-2+deb8u16.
- Uploaded [jackson-databind](https://tracker.debian.org/pkg/jackson-databind) to [buster-pu](https://bugs.debian.org/987489), fixing [CVE-2020-24616](https://security-tracker.debian.org/tracker/CVE-2020-24616), [CVE-2020-24750](https://security-tracker.debian.org/tracker/CVE-2020-24750), [CVE-2020-25649](https://security-tracker.debian.org/tracker/CVE-2020-25649), [CVE-2020-35490](https://security-tracker.debian.org/tracker/CVE-2020-35490), [CVE-2020-35491](https://security-tracker.debian.org/tracker/CVE-2020-35491), [CVE-2020-35728](https://security-tracker.debian.org/tracker/CVE-2020-35728), [CVE-2020-36179](https://security-tracker.debian.org/tracker/CVE-2020-36179), [CVE-2020-36180](https://security-tracker.debian.org/tracker/CVE-2020-36180), [CVE-2020-36181](https://security-tracker.debian.org/tracker/CVE-2020-36181), [CVE-2020-36182](https://security-tracker.debian.org/tracker/CVE-2020-36182), [CVE-2020-36183](https://security-tracker.debian.org/tracker/CVE-2020-36183), [CVE-2020-36184](https://security-tracker.debian.org/tracker/CVE-2020-36184), [CVE-2020-36185](https://security-tracker.debian.org/tracker/CVE-2020-36185), [CVE-2020-36186](https://security-tracker.debian.org/tracker/CVE-2020-36186), [CVE-2020-36187](https://security-tracker.debian.org/tracker/CVE-2020-36187), [CVE-2020-36188](https://security-tracker.debian.org/tracker/CVE-2020-36188), [CVE-2020-36189](https://security-tracker.debian.org/tracker/CVE-2020-36189), and [CVE-2021-20190](https://security-tracker.debian.org/tracker/CVE-2021-20190).  
  For Debian 10 buster, these problems have been fixed in version 2.9.8-3+deb10u3.
- Issued [ELA 404-1](https://deb.freexian.com/extended-lts/updates/ela-404-1-clamav/), fixing [CVE-2021-1405](https://security-tracker.debian.org/tracker/CVE-2021-1405), for [clamav](https://tracker.debian.org/pkg/clamav).  
  For Debian 8 jessie, these problems have been fixed in version 0.102.4+dfsg-0+deb8u2.
- Issued [ELA 409-1](https://deb.freexian.com/extended-lts/updates/ela-409-1-opendmarc/), fixing [CVE-2019-16378](https://security-tracker.debian.org/tracker/CVE-2019-16378) and [CVE-2020-12460](https://security-tracker.debian.org/tracker/CVE-2020-12460), for [opendmarc](https://tracker.debian.org/pkg/opendmarc).  
  For Debian 8 jessie, these problems have been fixed in version 1.3.0+dfsg-1+deb8u1.

#### Other (E)LTS Work:

- Front-desk duty from 29-03 until 04-04 and then from 26-04 until 02-05 for both LTS and ELTS.
- Triaged [spamassassin](https://tracker.debian.org/pkg/spamassassin),
[codemirror-js](https://tracker.debian.org/pkg/codemirror-js),
[jackson-databind](https://tracker.debian.org/pkg/jackson-databind),
[wordpress](https://tracker.debian.org/pkg/wordpress),
[gstreamer](https://tracker.debian.org/pkg/gstreamer),
[underscore](https://tracker.debian.org/pkg/underscore),
[python-bleach](https://tracker.debian.org/pkg/python-bleach),
[plinth](https://tracker.debian.org/pkg/plinth),
[libpano13](https://tracker.debian.org/pkg/libpano13),
[salt](https://tracker.debian.org/pkg/salt),
[dojo](https://tracker.debian.org/pkg/dojo),
[ruby2.7](https://tracker.debian.org/pkg/ruby2.7),
[firefox-esr](https://tracker.debian.org/pkg/firefox-esr),
[clamav](https://tracker.debian.org/pkg/clamav),
[composter](https://tracker.debian.org/pkg/composter),
[courier-authlib](https://tracker.debian.org/pkg/courier-authlib),
[opendmarc](https://tracker.debian.org/pkg/opendmarc),
[openexr](https://tracker.debian.org/pkg/openexr),
[libimage-exiftool-perl](https://tracker.debian.org/pkg/libimage-exiftool-perl),
[tomcat7](https://tracker.debian.org/pkg/tomcat7),
[libjs-handlebars](https://tracker.debian.org/pkg/libjs-handlebars),
[libnet-netmask-perl](https://tracker.debian.org/pkg/libnet-netmask-perl),
[network-manager](https://tracker.debian.org/pkg/network-manager), and
[curl](https://tracker.debian.org/pkg/curl).
- Mark CVE-2021-20297/network-manager as not-affected for jessie.
- Mark CVE-2021-22890/curl as not-affected for jessie and stretch.
- Mark CVE-2020-7760/codemirror-js as not-affected for jessie.
- Mark CVE-2021-25122/tomcat8 as not-affected for jessie.
- Mark CVE-2021-XXXX/plinth as no-dsa for stretch.
- Mark CVE-2021-29424/libnet-netmask-perl as no-dsa for stretch.
- Mark CVE-2021-28374/courier-authlib as fixed in 0.58-3.1 for jessie.
- Mark CVE-2021-1252/clamav as not-affected for jessie.
- Mark CVE-2021-1404/clamav as not-affected for jessie.
- Mark CVE-2020-4051/dojo as no-dsa for jessie.
- Mark CVE-2021-29447/wordpress as not-affected for jessie.
- Mark CVE-2021-29450/wordpress as not-affected for jessie.
- Mark CVE-2019-20920/libjs-handlebars as ignored for stretch and jessie.
- Mark CVE-2021-23369/libjs-handlebars as ignored for stretch and jessie.
- Mark CVE-2020-4051/dojo as fixed in 1.15.4+dfsg1-1 for sid and bullseye.
- Mark CVE-2021-28965/ruby2.7 fixed in 2.7.3-1 for sid.
- Mark CVE-2020-12272/opendmarc as postponed for jessie.
- Mark CVE-2021-20296, CVE-2021-3475, CVE-2021-3476, CVE-2021-3477, CVE-2021-3478, and CVE-2021-3479, affecting openexr, as no-dsa for jessie and stretch.
- Suggest proposed fixes for [CVE-2021-22876/curl on LTS public list](https://lists.debian.org/debian-lts/2021/04/msg00002.html).
- Publish the missing DLA update for the website on behalf of the community contribution. Thread [here](https://lists.debian.org/debian-lts/2021/04/msg00017.html).
- Help suggest and unblock work if FD is missing or something. Thread [here](https://lists.debian.org/debian-lts/2021/04/msg00009.html).
- Suggest marking CVE-2021-23369/{node,libjs}-handlebars as no-dsa/ignored for all suites. Thread [here](https://lists.debian.org/debian-lts/2021/04/msg00026.html).
- Help unblock Anton with the failed python2.7 build on i386 by coordinating with the sec team. Thread [here](https://lists.debian.org/debian-lts/2021/04/msg00034.html).
- Private ELTS-related discussion on the ELTS list (+ w/ Raphael).
- Auto EOL'ed webkit2gtk, python-bleach, tika, linux, ircii, spice-vdagent, libspring-security-2.0-java, file-roller, rustc, python-django-registration, gsoap, thunderbird, mosquitto, ruby-sidekiq, gnuchess, libpodofo, unbound, drupal7, 389-ds-base, and scrollz for jessie.
- Answered questions (& discussions) on IRC (#debian-lts and #debian-elts).
- General and other discussions on LTS private and [public mailing list](https://lists.debian.org/debian-lts/2021/02/threads.html).

---

Until next time.  
`:wq` for today.
