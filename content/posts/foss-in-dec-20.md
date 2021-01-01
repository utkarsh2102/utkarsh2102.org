+++
date = "2021-01-01 18:00:00 +0530"
title = "FOSS Activites in December 2020"
slug = "foss-in-dec-20"
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

Here's my (fifteenth) monthly update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 23rd month of contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March last year and a [DD](https://wiki.debian.org/DebianDeveloper) last Christmas! \o/

Apart from doing a bunch of activities like attending KubeCon + RubyConf (blog to follow!), et al and simultaneously giving
my undergrad exams, I did (relatively) more work than I had really anticipated!

Here are the following things I did in Debian this month:

#### Uploads and bug fixes:


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

- Issued [DLA 2474-1](https://lists.debian.org/debian-lts-announce/2020/11/msg00050.html), fixing [CVE-2020-28928](https://security-tracker.debian.org/tracker/CVE-2020-28928), for [musl](https://tracker.debian.org/pkg/musl).  
  For Debian 9 Stretch, these problems have been fixed in version 1.1.16-3+deb9u1.
- Issued [DLA 2481-1](https://lists.debian.org/debian-lts-announce/2020/12/msg00008.html), fixing [CVE-2020-25709](https://security-tracker.debian.org/tracker/CVE-2020-25709) and [CVE-2020-25710](https://security-tracker.debian.org/tracker/CVE-2020-25710), for [openldap](https://tracker.debian.org/pkg/openldap).  
  For Debian 9 Stretch, these problems have been fixed in version 2.4.44+dfsg-5+deb9u6.
- Issued [DLA 2484-1](https://lists.debian.org/debian-lts-announce/2020/12/msg00010.html), fixing [#969126](https://bugs.debian.org/969126), for [python-certbot](https://tracker.debian.org/pkg/python-certbot).  
  For Debian 9 Stretch, these problems have been fixed in version 0.28.0-1~deb9u3.
- Issued [DLA 2487-1](https://lists.debian.org/debian-lts-announce/2020/12/msg00013.html), fixing [CVE-2020-27350](https://security-tracker.debian.org/tracker/CVE-2020-27350), for [apt](https://tracker.debian.org/pkg/apt).  
  For Debian 9 Stretch, these problems have been fixed in version 1.4.11. The update was prepared by the maintainer, Julian.
- Issued [DLA 2488-1](https://lists.debian.org/debian-lts-announce/2020/12/msg00014.html), fixing [CVE-2020-27351](https://security-tracker.debian.org/tracker/CVE-2020-27351), for [python-apt](https://tracker.debian.org/pkg/python-apt).  
  For Debian 9 Stretch, these problems have been fixed in version 1.4.2. The update was prepared by the maintainer, Julian.
- Issued [DLA 2495-1](https://lists.debian.org/debian-lts-announce/2020/12/msg00022.html), fixing [CVE-2020-17527](https://security-tracker.debian.org/tracker/CVE-2020-17527), for [tomcat8](https://tracker.debian.org/pkg/tomcat8).  
  For Debian 9 Stretch, these problems have been fixed in version 8.5.54-0+deb9u5.
- Issued [DLA 2488-2](https://lists.debian.org/debian-lts-announce/2020/12/msg00037.html), for [python-apt](https://tracker.debian.org/pkg/python-apt).  
  For Debian 9 Stretch, these problems have been fixed in version 1.4.3. The update was prepared by the maintainer, Julian.
- Issued [DLA 2508-1](https://lists.debian.org/debian-lts-announce/2020/12/msg00038.html), fixing [CVE-2020-35730](https://security-tracker.debian.org/tracker/CVE-2020-35730), for [roundcube](https://tracker.debian.org/pkg/roundcube).  
  For Debian 9 Stretch, these problems have been fixed in version 1.2.3+dfsg.1-4+deb9u8. The update was prepared by the maintainer, Guilhem.

#### ELTS CVE Fixes and Announcements:

- Issued [ELA 324-1](https://deb.freexian.com/extended-lts/updates/ela-324-1-musl/), fixing [CVE-2020-28928](https://security-tracker.debian.org/tracker/CVE-2020-28928), for [musl](https://tracker.debian.org/pkg/musl).  
  For Debian 8 Jessie, these problems have been fixed in version 1.1.5-2+deb8u2.
- Issued [ELA 325-1](https://deb.freexian.com/extended-lts/updates/ela-325-1-mutt/), fixing [CVE-2020-28896](https://security-tracker.debian.org/tracker/CVE-2020-28896), for [mutt](https://tracker.debian.org/pkg/mutt).  
  For Debian 8 Jessie, these problems have been fixed in version 1.5.23-3+deb8u4.
- Issued [ELA 327-1](https://deb.freexian.com/extended-lts/updates/ela-327-1-openldap/), fixing [CVE-2020-25709](https://security-tracker.debian.org/tracker/CVE-2020-25709) and [CVE-2020-25710](https://security-tracker.debian.org/tracker/CVE-2020-25710), for [openldap](https://tracker.debian.org/pkg/openldap).  
  For Debian 8 Jessie, these problems have been fixed in version 2.4.40+dfsg-1+deb8u8.
- Issued [ELA 335-1](https://deb.freexian.com/extended-lts/updates/ela-335-1-flac/), fixing [CVE-2020-0499](https://security-tracker.debian.org/tracker/CVE-2020-0499), for [flac](https://tracker.debian.org/pkg/flac).  
  For Debian 8 Jessie, these problems have been fixed in version 1.3.0-3+deb8u1.
- Issued [ELA 340-1](https://deb.freexian.com/extended-lts/updates/ela-340-1-cairo/), fixing [CVE-2020-35492](https://security-tracker.debian.org/tracker/CVE-2020-35492), for [cairo](https://tracker.debian.org/pkg/cairo).  
  For Debian 8 Jessie, these problems have been fixed in version 1.14.0-2.1+deb8u3.

#### Other (E)LTS Work:


---

Until next time.  
`:wq` for today.
