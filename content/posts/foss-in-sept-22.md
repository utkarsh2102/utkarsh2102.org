+++
date = "2022-09-30 11:11:11 +0530"
title = "FOSS Activites in September 2022"
slug = "foss-in-sept-22"
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

Here's my (thirty-sixth) monthly but brief update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 45th month of actively contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March 2019 and a [DD](https://wiki.debian.org/DebianDeveloper) on Christmas '19! \o/

There's a bunch of things I do, both, technical and non-technical. Here are the things I did this month:

#### Debian Uploads

- [rails](https://tracker.debian.org/pkg/rails) (2:6.1.6.1+dfsg-2) - Add patch to allow Symbols in YAML columns, fixes [#1018934](https://bugs.debian.org/1018934).
- [rails](https://tracker.debian.org/pkg/rails) (2:6.1.6.1+dfsg-3) - Add patch to remove active_record.yaml initializers.
- [rails](https://tracker.debian.org/pkg/rails) (2:6.1.6.1+dfsg-4) - Add patch to allow Date, Time, ActiveSupport::HashWithIndifferentAccess in YAML columns.
- [ruby-arbre](https://tracker.debian.org/pkg/ruby-arbre) (1.4.0-2) - Add patch to use selector to detect authenticity token input.
- [ruby-net-http-digest-auth](https://tracker.debian.org/pkg/ruby-net-http-digest-auth) (1.4.1-1) - New upstream version, v1.4.1 to fix the FTBFS w/ rails.
- [rails](https://tracker.debian.org/pkg/rails) (2:6.1.7+dfsg-1) - New upstream version, v6.1.7+dfsg.
- [redmine](https://tracker.debian.org/pkg/redmine) (5.0.2-1) - New upstream version, v5.0.2 + fixes for [#1017525](https://bugs.debian.org/1017525), [#1019607](https://bugs.debian.org/1019607), [#1019238](https://bugs.debian.org/1019238), and [#1014813](https://bugs.debian.org/1014813).
- [redmine](https://tracker.debian.org/pkg/redmine) (5.0.2-2) - Add patch to relax pg's version for autopkgtest.
- [ruby-json-jwt](https://tracker.debian.org/pkg/ruby-json-jwt) (1.14.0-2) - No-change rebuild for unstable to fix [#1011682](https://bugs.debian.org/1011682).
- [libexporter-tiny-perl](https://tracker.debian.org/pkg/libexporter-tiny-perl) (1.004002-1) - New upstream version, v1.004002.

#### Other $things:

- Sponsored php-nikic-fast-route/1.3.0-4~bpo11+1 for William.
- Being an AM for [Arun Kumar, process #1024](https://nm.debian.org/process/1024/).
- Sponsoring stuff for non-DDs.
- Mentoring for newcomers.
- Moderation of -project mailing list.

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

This was my 20th month of actively contributing to [Ubuntu](https://ubuntu.com/about).
Now that I joined [Canonical to work on Ubuntu full-time](https://utkarsh2102.org/posts/hello-canonical/), there's a bunch of things I do! \o/

I mostly worked on different things, I guess.

I was too lazy to maintain a list of things I worked on so there's
no concrete list atm. Maybe I'll get back to this section later or
will start to list stuff from the fall, as I was doing before. :D

---

## Debian (E)LTS
{{< figure src="/images/debian-lts-small.png" >}}

[Debian Long Term Support (LTS)](https://www.freexian.com/en/services/debian-lts.html) is a project to extend the lifetime of all Debian stable releases to (at least) 5 years. Debian LTS is not handled by the Debian security team, but by a separate group of volunteers and companies interested in making it a success.  

And [Debian Extended LTS (ELTS)](https://deb.freexian.com/extended-lts) is its sister project, extending support to the Jessie release (+2 years after LTS support).

This was my thirty-sixth month as a Debian LTS and twenty-seventh month as a Debian ELTS paid contributor.  
I worked for 38.00 hours for LTS and 27.00 hours for ELTS.

#### LTS CVE Fixes and Announcements:

- Rolled out announcement for src:flac.
- Rolled out announcement for src:ruby-rack.
- Issued [DLA 3128-1](https://lists.debian.org/debian-lts-announce/2022/09/msg00039.html), fixing [CVE-2020-7677](https://security-tracker.debian.org/tracker/CVE-2020-7677), for [node-thenify](https://tracker.debian.org/pkg/node-thenify).  
  For Debian 10 buster, these problems have been fixed in version 3.3.0-1+deb10u1.
- Issued [DLA 3129-1](https://lists.debian.org/debian-lts-announce/2022/09/msg00040.html), fixing [CVE-2019-17545](https://security-tracker.debian.org/tracker/CVE-2019-17545) and [CVE-2021-45943](https://security-tracker.debian.org/tracker/CVE-2021-45943), for [gdal](https://tracker.debian.org/pkg/gdal).  
  For Debian 10 buster, these problems have been fixed in version 2.4.0+dfsg-1+deb10u1.
- Looked at src:mbedtls which has about 18 CVEs opened in buster (including no-dsa).  
  Also, spoke to the maintainer - they said they'd be uncomfortable doing or reviewing the backport (although they initially said they'd be happy to help).
- Fixed src:rails regression via 2:6.1.6.1+dfsg-2, 2:6.1.6.1+dfsg-3, and 2:6.1.6.1+dfsg-4 for sid.  
  CVE-2022-32224 broke the entire world. :)
- Helped Abhijith figure out the regression fix for CVE-2022-32224.  
  Also got that verified by the people who reported regression, [Raphael](https://lists.debian.org/debian-lts/2022/09/msg00024.html), [Sven](https://lists.debian.org/debian-lts/2022/09/msg00037.html), and [Jude](https://lists.debian.org/debian-lts/2022/09/msg00045.html). The whole thread is on debian-lts@.

#### ELTS CVE Fixes and Announcements:

- Rolled out announcemnet for src:ruby-tzinfo.
- Rolled out announcemnet for src:grubt.
- Issued [ELA 682-1](https://www.freexian.com/lts/extended/updates/ela-682-1-open-vm-tools/), fixing [CVE-2022-31676](https://security-tracker.debian.org/tracker/CVE-2022-31676), for [open-vm-tools](https://tracker.debian.org/pkg/open-vm-tools).  
  For Debian 9 stretch, these problems have been fixed in version 2:10.1.5-5055683-4+deb9u3.
- Issued [ELA 691-1](https://www.freexian.com/lts/extended/updates/ela-691-1-wkhtmltopdf/), fixing [CVE-2020-21365](https://security-tracker.debian.org/tracker/CVE-2020-21365), for [wkhtmltopdf](https://tracker.debian.org/pkg/wkhtmltopdf).  
  For Debian 8 jessie, these problems have been fixed in version 0.12.1-2+deb8u1.  
  For Debian 9 stretch, these problems have been fixed in version 0.12.3.2-3+deb9u1.
- Issued [ELA 692-1](), fixing [CVE-2022-37452](https://security-tracker.debian.org/tracker/CVE-2022-37452), for [exim4](https://tracker.debian.org/pkg/exim4).  
  For Debian 8 jessie, these problems have been fixed in version 4.84.2-2+deb8u9.  
  For Debian 9 stretch, these problems have been fixed in version 4.89-2+deb9u9.
- Started to look at src:tiff again. Has a lot of open issues. Haven't claimed the package officially yet, though. :)

#### Other (E)LTS Work:

- Triaged [rails](https://tracker.debian.org/pkg/rails),
[node-thenify](https://tracker.debian.org/pkg/node-thenify),
[exim4](https://tracker.debian.org/pkg/exim4),
[wkhtmltopdf](https://tracker.debian.org/pkg/wkhtmltopdf),
[gdal](https://tracker.debian.org/pkg/gdal), and
[mbedtls](https://tracker.debian.org/pkg/mbedtls).
- Marked CVE-2019-25050/gdal as not-affected for buster.
- Marked CVE-2022-37451/exim4 as not-affected for stretch and jessie; following buster and bullseye.
- Helped and assisted new contributors joining Freexian (LTS/ELTS).
- Answered questions (& discussions) on IRC (#debian-lts and #debian-elts) and Matrix.
- Participated and helped fellow members with their queries via private mail and chat.
- General and other discussions on LTS private and [public mailing list](https://lists.debian.org/debian-lts/2022/09/threads.html).
- Attended the monthly public meeting held on #debian-lts on September 29th.

---

Until next time.  
`:wq` for today.
