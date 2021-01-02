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

This was my 24th month of contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March last year and a [DD](https://wiki.debian.org/DebianDeveloper) last Christmas! \o/

Amongs a lot of things, this was month was crazy, hectic, adventerous, and the last of 2020 -- more on some parts later this month.  
I finally finished my 7th semester (FTW!) and moved onto my last one! That said, I had been busy with other things™ but still did a bunch of Debian stuff

Here are the following things I did this month:

#### Uploads and bug fixes:

- [ruby-gh](https://tracker.debian.org/pkg/ruby-gh) (0.18.0-2) - .
- [ruby-gh](https://tracker.debian.org/pkg/ruby-gh) (0.18.0-3) - .
- [libgit2](https://tracker.debian.org/pkg/libgit2) (1.0.1+dfsg.1-2) - .
- [libgit2](https://tracker.debian.org/pkg/libgit2) (1.0.1+dfsg.1-3) - .
- [libgit-raw-perl](https://tracker.debian.org/pkg/libgit-raw-perl) (0.87+ds-1) - .
- [python-pygit2](https://tracker.debian.org/pkg/python-pygit2) (1.3.0+dfsg1-2) - .
- [golang-gopkg-libgit2-git2go.v30](https://tracker.debian.org/pkg/golang-gopkg-libgit2-git2go.v30) (30.3.2-1) - .
- [libgit2](https://tracker.debian.org/pkg/libgit2) (1.1.0+dfsg.1-1) - .
- [golang-gopkg-libgit2-git2go.v30](https://tracker.debian.org/pkg/golang-gopkg-libgit2-git2go.v30) (30.3.2-2) - .
- [golang-gopkg-libgit2-git2go.v31](https://tracker.debian.org/pkg/golang-gopkg-libgit2-git2go.v31) (31.4.3-1) - .
- [libgit2](https://tracker.debian.org/pkg/libgit2) (1.1.0+dfsg.1-2) - .
- [python-pygit2](https://tracker.debian.org/pkg/python-pygit2) (1.4.0+dfsg1-1) - .
- [ruby-rugged](https://tracker.debian.org/pkg/ruby-rugged) (1.1.0+ds-1) - .
- [rails](https://tracker.debian.org/pkg/rails) (2:6.0.3.4+dfsg-2) - .
- [ruby3.0](https://tracker.debian.org/pkg/ruby3.0) (3.0.0~preview2-1) - .
- [golang-gopkg-libgit2-git2go.v31](https://tracker.debian.org/pkg/golang-gopkg-libgit2-git2go.v31) (31.4.3-2) - .
- [golang-github-robertkrimen-otto](https://tracker.debian.org/pkg/golang-github-robertkrimen-otto) (0.0~git20200922.ef014fd-1) - .
- [bidi-clojure](https://tracker.debian.org/pkg/bidi-clojure) (2.1.3-2) - .
- [comidi-clojure](https://tracker.debian.org/pkg/comidi-clojure) (0.3.2-2) - .
- [ruby3.0](https://tracker.debian.org/pkg/ruby3.0) (3.0.0~rc1-1) - .
- [polybar](https://tracker.debian.org/pkg/polybar) (3.5.3-1) - .
- [ruby3.0](https://tracker.debian.org/pkg/ruby3.0) (3.0.0-1) - .
- [pathetic-clojure](https://tracker.debian.org/pkg/pathetic-clojure) (0.5.1-2) - .
- [url-clojure](https://tracker.debian.org/pkg/url-clojure) (0.1.1-2) - .
- [libgit2](https://tracker.debian.org/pkg/libgit2) (1.1.0+dfsg.1-3) - .
- [ruby-paper-trail](https://tracker.debian.org/pkg/ruby-paper-trail) (11.1.0-1) - .

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

This was my fifteenth month as a Debian LTS and sixth month as a Debian ELTS paid contributor.  
I was assigned 26.00 hours for LTS and 38.25 hours for ELTS and worked on the following things:  

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

- Front-desk duty from 21-12 until 27-12 and from 28-12 until 03-01 for both LTS and ELTS.
- Triaged [openldap](https://tracker.debian.org/pkg/openldap),
[python-certbot](https://tracker.debian.org/pkg/python-certbot),
[lemonldap-ng](https://tracker.debian.org/pkg/lemonldap-ng),
[qemu](https://tracker.debian.org/pkg/qemu),
[gdm3](https://tracker.debian.org/pkg/gdm3),
[open-iscsi](https://tracker.debian.org/pkg/open-iscsi),
[gobby](https://tracker.debian.org/pkg/gobby),
[jackson-databind](https://tracker.debian.org/pkg/jackson-databind),
[wavpack](https://tracker.debian.org/pkg/wavpack),
[cairo](https://tracker.debian.org/pkg/cairo),
[nsd](https://tracker.debian.org/pkg/nsd),
[tomcat8](https://tracker.debian.org/pkg/tomcat8), and
[bountycastle](https://tracker.debian.org/pkg/bountycastle).
- Marked CVE-2020-17527/tomcat8 as not-affected for jessie.
- Marked CVE-2020-28052/bountycastle as not-affected for jessie.
- Marked CVE-2020-14394/qemu as postponed for jessie.
- Marked CVE-2020-35738/wavpack as not-affected for jessie.
- Marked CVE-2020-3550{3-6}/qemu as postponed for jessie.
- Marked CVE-2020-3550{3-6}/qemu as postponed for stretch.
- Marked CVE-2020-16093/lemonldap-ng as no-dsa for stretch.
- Marked CVE-2020-27837/gdm3 as no-dsa for stretch.
- Marked CVE-2020-{13987, 13988, 17437}/open-iscsi as no-dsa for stretch.
- Marked CVE-2020-35450/gobby as no-dsa for stretch.
- Marked CVE-2020-35728/jackson-databind as no-dsa for stretch.
- Marked CVE-2020-28935/nsd as no-dsa for stretch.
- Auto EOL'ed libpam-tacplus, open-iscsi, wireshark, gdm3, golang-go.crypto, jackson-databind, spotweb, python-autobahn, asterisk, nsd, ruby-nokogiri, linux, and motion for jessie.
- General discussion on LTS private and [public mailing list](https://lists.debian.org/debian-lts/2020/12/threads.html).

---

Until next time.  
`:wq` for today.