+++
date = "2019-12-30"
title = "FOSS Activites in December 2019"
slug = "foss-in-dec-19"
tags = [
    "debian",
    "monthly",
]
categories = [
    "debian",
    "open-source",
]
+++

Here's my (third) monthly update about the activities I've done in Debian this December.

## Debian LTS

This was my third month as a Debian LTS paid contributor.  
I was assigned 16.50 hours and worked on the following things:  

#### CVE Fixes and Announcements:

- Issued [DLA 2024-1](https://lists.debian.org/debian-lts-announce/2019/12/msg00006.html), fixing CVE-2019-19617, for phpmyadmin.  
  Details here:
  >  phpMyAdmin before 4.9.2 does not escape certain Git information, related to libraries/display_git_revision.lib.php and libraries/Footer.class.php.  

  For Debian 8 "Jessie", this has been fixed in 4:4.2.12-2+deb8u7.  
  Furthermore, sent a patch to the Security team for fixing the same in Stretch.  

- Issued [DLA 2025-1](https://lists.debian.org/debian-lts-announce/2019/12/msg00007.html), fixing CVE-2017-17833 and CVE-2019-5544, for openslp-dfsg.  
  Details here:
  > OpenSLP releases in the 1.0.2 and 1.1.0 code streams have a heap-related memory corruption issue which may manifest itself as a denial-of-service
    or a remote code-execution vulnerability.  
    OpenSLP as used in ESXi and the Horizon DaaS appliances has a heap overwrite issue. VMware has evaluated the severity of this issue to be in
    the critical severity range.

  For Debian 8 "Jessie", this has been fixed in 1.2.1-10+deb8u2.  

- Issued [DLA 2026-1](https://lists.debian.org/debian-lts-announce/2019/12/msg00008.html), fixing CVE-2019-19630, for htmldoc.  
  Details here:
  > In HTMLDOC, there was a one-byte underflow in htmldoc/ps-pdf.cxx caused by a floating point math difference between GCC and Clang.  

  For Debian 8 "Jessie", this has been fixed in 1.8.27-8+deb8u1.  
  Furthermore, sent a patch to the Security team for Stretch and Buster.  

- Issued [DLA 2046-1](https://lists.debian.org/debian-lts-announce/2019/12/msg00031.html), fixing CVE-2019-19479, for opensc.  
  Details here:
  > An issue was discovered in libopensc/card-setcos.c in OpenSC, which has an incorrect read operation during parsing of a SETCOS file attribute.  

  For Debian 8 "Jessie", this has been fixed in 0.16.0-3+deb8u2.  

#### Miscellaneous:

- Triage [luajit](https://tracker.debian.org/pkg/luajit), [python-oslo.utils](https://tracker.debian.org/pkg/python-oslo.utils), [davical](https://tracker.debian.org/pkg/davical), [sqlite3](https://tracker.debian.org/pkg/sqlite3), [phpmyadmin](https://tracker.debian.org/pkg/phpmyadmin), [openssl](https://tracker.debian.org/pkg/openssl), [htmldoc](https://tracker.debian.org/pkg/htmldoc), and [opensc](https://tracker.debian.org/pkg/opensc) for Jessie.  

- Pinged upstream of [libexif](https://tracker.debian.org/pkg/libexif), [ruby-rack](https://tracker.debian.org/pkg/ruby-rack), and [ruby-rack-cors](https://tracker.debian.org/pkg/ruby-rack-cors) for more clarification of the patches provided.  

- Clarified more about CVE-2019-1551/openssl triage to the Security Team and the Debian LTS [ML](https://lists.debian.org/debian-lts/2019/12/msg00028.html).  

- Took a deeper look at CVE-2019-16782/ruby-rack; the patch itself introduces regression and induces a backdoor on its own. Notified the Security Team and the [ML](https://lists.debian.org/debian-lts/2019/12/msg00050.html) to avoid its upload.  

- Discuss the state of CVE-2019-19479/opensc with Roberto and process its upload. Also opened [upstream issue](https://github.com/google/oss-fuzz/issues/3132) out of frustration for "hiding" most of their report.  

- In midst of fixing test failures of ruby-rack-cores. And also WIP for ruby-excon.  

---

## Debian Uploads

Most importantly, I became a DD this month! \o/  
Here's my [NM process](https://nm.debian.org/process/682). Many, many thanks to Thomas (zigo) for being so nice and patient! :D   

#### Uploads to the Archive:

- ruby-reverse-markdown ~ 1.3.0-1 (to unstable).  
- ruby-behance ~ 0.6.1-1 (to unstable).  
- ruby-unidecode ~ 1.0.0-1 (to unstable).  
- micro ~ 1.4.1-1 (to unstable).  
- golang-code.cloudfoundry-bytefmt ~ 0.0~git20190818.854d396-1 (to unstable).  
- micro ~ 1.4.1-2 (to unstable).  
- golang-github-flynn-json5 ~ 0.0~git20160717.7620272-2 (to unstable).  
- golang-github-zyedidia-pty ~ 1.1.1+git20180126.3036466-2 (to unstable).  
- golang-github-zyedidia-terminal ~ 0.0~git20180726.533c623-2 (to unstable).  
- golang-golang-x-text ~ 0.3.2-3 (to unstable).  
- golang-github-yuin-gopher-lua ~ 0.0~git20170915.0.eb1c729-4 (to unstable).  
- golang-github-sergi-go-diff ~ 1.0.0-2 (to unstable).  

#### Bug Fixes:

- #946859 for ruby-reverse-markdown (ITP).  
- #946895 for ruby-behance (ITP).  
- #946945 for ruby-unidecode (ITP).  
- #947724 for golang-code.cloudfoundry-bytefmt (ITP).  
- #889196 for golang-github-yuin-gopher-lua.  
- #889209 for golang-github-sergi-go-diff.  

#### Reviews and Sponsored Uploads:

- easygen ~ 4.1.0-1 for Tong Sun.  
- node-webpack ~ 4.30.0-1 for Pirate Praveen.
- node-timeago.js ~ 4.0.2-1 for Sakshi Sangwan.  

##### Miscellaneous:

- Outreachy mentoring for GitLab project.  
- Grant DM access for easygen to Tong Sun.  
- Grant DM access for golang-github-danverbraganza-varcaser to Tong Sun.  
- Help James Montgomery for Golang packaging (wrt [#945524](https://bugs.debian.org/cgi-bin/bugreport.cgi?bug=945524)).  
- Migrated all my -guest accounts and certificates to use my new, shiny account associated with the DD status.  
- With regards to [this tweet](https://twitter.com/utkarsh2102/status/1166908945614561281), I assisted the following people:  
    - Shubhank Saxena with 1:1 Hangouts call.  
    - Shreya Gupta with 1:1 Hangouts call.  
    - Eshaan Bansal with 1:1 Hangouts call.  
    P.S. It was lovely to interact with such lovely people :)  

---

Until next time.  
`:wq` for today.
