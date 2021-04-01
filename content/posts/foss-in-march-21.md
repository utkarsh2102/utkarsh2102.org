+++
date = "2021-04-01 12:00:00 +0530"
title = "FOSS Activites in March 2021"
slug = "foss-in-march-21"
images = [
    "/images/debian-logo-small.png",
    "/images/debian_ruby.png",
    "/images/ruby-logo-small.png",
    "/images/debian-lts-small.png",
    "/images/computing.jpg",
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

Here's my (eighteenth) monthly update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 27th month of active contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March 2019 and a [DD](https://wiki.debian.org/DebianDeveloper) on Christmas '19! \o/

This month was a bit exhausting; lots of moving parts. With the financial year ending, it was even more crazy, with me running around to banks, CA, et al.  
Anyway, with now working on Ubuntu full-time, I did little of Debian this month. Here are the following things I worked on:

#### Uploads and bug fixes:

- [polybar](https://tracker.debian.org/pkg/polybar) (3.5.5-1) - New upstream version, v3.5.5.
- [ruby-http-parser](https://tracker.debian.org/pkg/ruby-http-parser) (1.2.1-5) - Disable tests causing FTBFS on s390x architecture.
- [debian-security-support](https://tracker.debian.org/pkg/debian-security-support) (1:11+2021.03.19) - Fix for [bug #984539](https://bugs.debian.org/984539): dpkg hook should never fail.
- Filed [bug #985314](https://bugs.debian.org/985314) against asterisk (systemd misconfiguration) and added a patch as well.
- Filed [bug #985421](https://bugs.debian.org/985421) against at (add DEP8 tests) and added a patch as well.

#### Other $things:

- Attended the Debian LTS team meeting.
- Mentoring for newcomers.
- Moderation of -project mailing list.

---

## Debian (E)LTS
{{< figure src="/images/debian-lts-small.png" >}}

[Debian Long Term Support (LTS)](https://www.freexian.com/en/services/debian-lts.html) is a project to extend the lifetime of all Debian stable releases to (at least) 5 years. Debian LTS is not handled by the Debian security team, but by a separate group of volunteers and companies interested in making it a success.  

And [Debian Extended LTS (ELTS)](https://deb.freexian.com/extended-lts) is its sister project, extending support to the Jessie release (+2 years after LTS support).

This was my eighteenth month as a Debian LTS and ninth month as a Debian ELTS paid contributor.  
I was assigned 60.00 hours for LTS and 39.00 hours for ELTS and worked on the following things:  

#### LTS CVE Fixes and Announcements:

- Issued [DLA 2580-1](https://lists.debian.org/debian-lts-announce/2021/03/msg00002.html), fixing [CVE-2021-21311](https://security-tracker.debian.org/tracker/CVE-2021-21311), for [adminer](https://tracker.debian.org/pkg/adminer).  
  For Debian 9 stretch, these problems have been fixed in version 4.2.5-3+deb9u2.
- Issued [DLA 2581-1](https://lists.debian.org/debian-lts-announce/2021/03/msg00003.html), fixing [CVE-2021-27803](https://security-tracker.debian.org/tracker/CVE-2021-27803), for [wpa](https://tracker.debian.org/pkg/wpa).  
  For Debian 9 stretch, these problems have been fixed in version 2:2.4-1+deb9u9.
- Issued [DLA 2585-1](https://lists.debian.org/debian-lts-announce/2021/03/msg00007.html), fixing [CVE-2020-13848](https://security-tracker.debian.org/tracker/CVE-2020-13848), for [libupnp](https://tracker.debian.org/pkg/libupnp).  
  For Debian 9 stretch, these problems have been fixed in version 1:1.6.19+git20160116-1.2+deb9u1.
- Issued [DLA 2589-1](https://lists.debian.org/debian-lts-announce/2021/03/msg00012.html), fixing [CVE-2020-26519](https://security-tracker.debian.org/tracker/CVE-2020-26519) and [CVE-2021-3407](https://security-tracker.debian.org/tracker/CVE-2021-3407), for [mupdf](https://tracker.debian.org/pkg/mupdf).  
  For Debian 9 stretch, these problems have been fixed in version 1.9a+ds1-4+deb9u6.
- Issued [DLA 2593-1](https://lists.debian.org/debian-lts-announce/2021/03/msg00016.html), fixing [bug #962596](https://bugs.debian.org/962596), for [ca-certificates](https://tracker.debian.org/pkg/ca-certificates).  
  For Debian 9 stretch, these problems have been fixed in version 20200601~deb9u2.
- Issued [DLA 2589-2](https://lists.debian.org/debian-lts-announce/2021/03/msg00017.html), fixing regression caused by DLA 2589-1, for [mupdf](https://tracker.debian.org/pkg/mupdf).  
  For Debian 9 stretch, these problems have been fixed in version 1.9a+ds1-4+deb9u7.
- Issued [DLA 2598-1](https://lists.debian.org/debian-lts-announce/2021/03/msg00022.html), fixing [CVE-2020-25097](https://security-tracker.debian.org/tracker/CVE-2020-25097), for [squid3](https://tracker.debian.org/pkg/squid3).  
  For Debian 9 stretch, these problems have been fixed in version 3.5.23-5+deb9u6.
- Issued [DLA 2599-1](https://lists.debian.org/debian-lts-announce/2021/03/msg00023.html), fixing [CVE-2021-28963](https://security-tracker.debian.org/tracker/CVE-2021-28963), for [shibboleth-sp2](https://tracker.debian.org/pkg/shibboleth-sp2).  
  For Debian 9 stretch, these problems have been fixed in version 2.6.0+dfsg1-4+deb9u2.
- Issued [DLA 2601-1](https://lists.debian.org/debian-lts-announce/2021/03/msg00025.html), fixing [CVE-2021-3429](https://security-tracker.debian.org/tracker/CVE-2021-3429), for [cloud-init](https://tracker.debian.org/pkg/cloud-init).  
  For Debian 9 stretch, these problems have been fixed in version 0.7.9-2+deb9u1.
- Issued [DLA 2558-2](https://lists.debian.org/debian-lts-announce/2021/03/msg00026.html), fixing regression caused by DLA 2558-1, for [xterm](https://tracker.debian.org/pkg/xterm).  
  For Debian 9 stretch, these problems have been fixed in version 327-2+deb9u2.
- Released [debian-security-support to unstable](https://tracker.debian.org/news/1236782/accepted-debian-security-support-11120210319-source-into-unstable/) via Holger to fix [bug #984539](https://bugs.debian.org/984539).

#### ELTS CVE Fixes and Announcements:

- Issued [ELA 374-1](https://deb.freexian.com/extended-lts/updates/ela-374-1-wpa/), fixing [CVE-2021-27803](https://security-tracker.debian.org/tracker/CVE-2021-27803), for [wpa](https://tracker.debian.org/pkg/wpa).  
  For Debian 8 jessie, these problems have been fixed in version 2.3-1+deb8u13.
- Issued [ELA 375-1](https://deb.freexian.com/extended-lts/updates/ela-375-1-libcaca/), fixing [CVE-2021-3410](https://security-tracker.debian.org/tracker/CVE-2021-3410), for [libcaca](https://tracker.debian.org/pkg/libcaca).  
  For Debian 8 jessie, these problems have been fixed in version 0.99.beta19-2+deb8u2.
- Issued [ELA 376-1](https://deb.freexian.com/extended-lts/updates/ela-376-1-libhibernate3-java/), fixing [CVE-2020-25638](https://security-tracker.debian.org/tracker/CVE-2020-25638), for [libhibernate3-java](https://tracker.debian.org/pkg/libhibernate3-java).  
  For Debian 8 jessie, these problems have been fixed in version 3.6.10.Final-3+deb8u1.
- Issued [ELA 382-1](https://deb.freexian.com/extended-lts/updates/ela-382-1-squid3/), fixing [CVE-2020-25097](https://security-tracker.debian.org/tracker/CVE-2020-25097), for [squid3](https://tracker.debian.org/pkg/squid3).  
  For Debian 8 jessie, these problems have been fixed in version 3.5.23-5+deb8u3.
- Issued [ELA 385-1](https://deb.freexian.com/extended-lts/updates/ela-385-1-shibboleth-sp2/), fixing [CVE-2021-28963](https://security-tracker.debian.org/tracker/CVE-2021-28963), for [shibboleth-sp2](https://tracker.debian.org/pkg/shibboleth-sp2).  
  For Debian 8 jessie, these problems have been fixed in version 2.5.3+dfsg-2+deb8u2.
- Issued [ELA 363-2](https://deb.freexian.com/extended-lts/updates/ela-363-2-xterm/), fixing regression caused by ELA 363-1, for [xterm](https://tracker.debian.org/pkg/xterm).  
  For Debian 8 jessie, these problems have been fixed in version 312-2+deb8u2.

#### Other (E)LTS Work:

- Front-desk duty from 01-03 until 07-03 for ELTS and then from 29-03 until 04-04 for both LTS and ELTS.
- Triaged [wpa](https://tracker.debian.org/pkg/wpa),
[python-aiohttp](https://tracker.debian.org/pkg/python-aiohttp),
[spip](https://tracker.debian.org/pkg/spip),
[wpa](https://tracker.debian.org/pkg/wpa),
[qemu](https://tracker.debian.org/pkg/qemu),
[tomcat7](https://tracker.debian.org/pkg/tomcat7),
[tomcat8](https://tracker.debian.org/pkg/tomcat8),
[grub2](https://tracker.debian.org/pkg/grub2),
[mupdf](https://tracker.debian.org/pkg/mupdf),
[openssh](https://tracker.debian.org/pkg/openssh),
[tiff](https://tracker.debian.org/pkg/tiff),
[spice](https://tracker.debian.org/pkg/spice),
[pillow](https://tracker.debian.org/pkg/pillow),
[xmlgraphics-commons](https://tracker.debian.org/pkg/xmlgraphics-commons),
[batik](https://tracker.debian.org/pkg/batik),
[libupnp](https://tracker.debian.org/pkg/libupnp),
[ca-certificates](https://tracker.debian.org/pkg/ca-certificates),
[salt](https://tracker.debian.org/pkg/salt),
[squid3](https://tracker.debian.org/pkg/squid3),
[shibboleth-sp2](https://tracker.debian.org/pkg/shibboleth-sp2),
[courier-authlib](https://tracker.debian.org/pkg/courier-authlib),
[cloud-init](https://tracker.debian.org/pkg/cloud-init),
[spamassassin](https://tracker.debian.org/pkg/spamassassin),
[openssl](https://tracker.debian.org/pkg/openssl),
[libcaca](https://tracker.debian.org/pkg/libcaca), and
[openjpeg2](https://tracker.debian.org/pkg/openjpeg2).
- Marked CVE-2021-21330/python-aiohttp as not-affected for stretch.
- Marked CVE-2021-20233, CVE-2021-20225, CVE-2020-27779, CVE-2020-27778, CVE-2020-27749, CVE-2020-27748, CVE-2020-25647, CVE-2020-25632, CVE-2020-25631, and CVE-2020-14372, affecting grub2, as ignored for stretch and jessie.
- Marked CVE-2020-27842/openjpeg2 as no-dsa for jessie.
- Marked CVE-2020-27843/openjpeg2 as no-dsa for jessie.
- Marked CVE-2021-28041/openssh as not-affect for jessie.
- Marked CVE-2020-3552{3,4}/tiff as no-dsa for jessie.
- Marked CVE-2021-20201/spice as no-dsa for jessie.
- Marked CVE-2020-11988/xmlgraphics-commons as postponed for jessie.
- Marked CVE-2020-11987/batik as postponed for jessie.
- Marked CVE-2020-12695/libupnp as no-dsa for stretch.
- Marked CVE-2021-25122/tomcat7 as not-affected for stretch.
- Marked CVE-2021-25329/tomcat7 as ignored for stretch.
- Marked CVE-2021-28116/squid3 as postponed for stretch and jessie.
- Marked CVE-2021-3449/openssl as not-affected for stretch.
- Document extra notes for grub2 for LTS and co-ordinate with the sec-team.
- Document extra notes for pillow about piled-up issues in jessie.
- Issued DLA-2593-1 for ca-certificates on Microsoft's request; co-ordinating w/ them.
- Co-ordinating w/ maintainer of courier-authlib for stretch and jessie update.
- Fixing build failures of ELTS' security tracker and re-ordering entries in data/CVE-EXTENDED-LTS/list file.
- Answer queries of dupondje and mikap about openssl on IRC; and it being not-affected for stretch.
- Help review the status of CVE-2021-3121/golang-github-gogo-protobuf-dev for Ola.
- Co-ordinating w/ Noah for cloud-init and setuptools.
- Auto EOL'ed mongodb, linux, guacamole-client, node-xmlhttprequest, newlib, neutron, privoxy, glpi, and zabbix for jessie.
- Attended monthly meeting for Debian LTS.
- Answered questions (& discussions) on IRC (#debian-lts and #debian-elts).
- General and other discussions on LTS private and [public mailing list](https://lists.debian.org/debian-lts/2021/03/threads.html).

---

Until next time.  
`:wq` for today.
