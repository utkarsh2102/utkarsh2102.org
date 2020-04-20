+++
date = "2020-02-01"
title = "FOSS Activites in January 2020"
slug = "foss-in-jan-20"
tags = [
    "debian",
    "monthly",
]
categories = [
    "debian",
    "open-source",
]
+++

Here's my (fourth) monthly update about the activities I've done in Debian this January.

## Debian LTS

This was my fourth month as a Debian LTS paid contributor.  
I was assigned 23.75 hours and worked on the following things:  

#### CVE Fixes and Announcements:

- Issued [DLA 2060-1](https://lists.debian.org/debian-lts-announce/2020/01/msg00011.html), fixing CVE-2020-5504, for phpmyadmin.  
  Details here:
  >  In phpMyAdmin 4 before 4.9.4 and 5 before 5.0.1, SQL injection exists in the user accounts page. A malicious user could inject custom SQL in place of their own username when creating queries to this page. An attacker must have a valid MySQL account to access the server.  

  For Debian 8 "Jessie", this problem has been fixed in version 4:4.2.12-2+deb8u8.  
  Furthermore, worked on preparing the security update for Stretch and Buster with the original maintainer.  

- Issued [DLA 2063-1](https://lists.debian.org/debian-lts-announce/2020/01/msg00012.html), fixing CVE-2019-3467 for debian-lan-config.  
  Details here:
  > In debian-lan-config < 0.26, configured too permissive ACLs for the Kerberos admin server allowed password changes for other Kerberos user principals.  

  For Debian 8 "Jessie", this problem has been fixed in version 0.19+deb8u2.  

- Issued [DLA 2070-1](https://lists.debian.org/debian-lts-announce/2020/01/msg00015.html), fixing CVE-2019-16779, for ruby-excon.  
  Details here:
  > In RubyGem excon before 0.71.0, there was a race condition around persistent connections, where a connection which is interrupted (such as by a timeout) would leave data on the socket. Subsequent requests would then read this data, returning content from the previous response.

  For Debian 8 "Jessie", this problem has been fixed in version 0.33.0-2+deb8u1.  
  Furthermore, sent a patch to the Security team for Stretch and Buster.  

  P.S. this backporting took the most time and effort this month.

- Issued [DLA 2090-1](https://lists.debian.org/debian-lts-announce/2020/01/msg00036.html), fixing CVE-2020-7039, for qemu.  
  Details here:
  > tcp_emu in tcp_subr.c in libslirp 4.1.0, as used in QEMU 4.2.0, mismanages memory, as demonstrated by IRC DCC commands in EMU_IRC. This can cause a heap-based buffer overflow or other out-of-bounds access which can lead to a DoS or potential execute arbitrary code.  

  For Debian 8 "Jessie", this problem has been fixed in version 1:2.1+dfsg-12+deb8u13.  

#### Miscellaneous:

- Triaged [samba](https://tracker.debian.org/pkg/samba), [cacti](https://tracker.debian.org/pkg/cacti), [storebackup](https://tracker.debian.org/pkg/storebackup), and [qemu](https://tracker.debian.org/pkg/qemu).  

- Checked with upstream of [ruby-rack](https://tracker.debian.org/pkg/ruby-rack) for their CVE fix which induces regression.  

- Worked a bit on [ruby-rack-cors](https://tracker.debian.org/pkg/ruby-rack-cors) but couldn't complete because of Amsterdam -> Brussels travel. Thanks to Brian for completing it \o/  

---

## Debian Uploads

This was a great month! MiniDebCamp -> FOSDEM -> Ruby Sprints. Blog post soon :D  
In any case, in the month of January, I did the following work:

#### Uploads to the Archive:

- ruby-haml-rails ~ 2.0.1-1 (to unstable).  
- golang-github-zyedidia-pty ~ 1.1.1+git20180126.3036466-3 (to unstable).  
- ruby-benchmark-suite ~ 1.0.0+git.20130122.5bded6-3 (to unstable).  
- golang-github-robertkrimen-otto ~ 0.0+git20180617.15f95af-2~bpo10+1 (to buster-backports).  
- golang-github-zyedidia-pty ~ 1.1.1+git20180126.3036466-3~bpo10+1 (to buster-backports).  
- golang-github-mitchellh-go-homedir ~ 1.1.0-1~bpo10+1 (to buster-backports).  
- golang-golang-x-sys ~ 0.0+git20190726.fc99dfb-1~bpo10+1 (to buster-backports).  
- golang-github-mattn-go-isatty ~ 0.0.8-2~bpo10+1 (to buster-backports).  
- golang-github-mattn-go-runewidth ~ 0.0.7-1~bpo10+1 (to buster-backports).  
- golang-github-dustin-go-humanize ~ 1.0.0-1~bpo10+1 (to buster-backports).  
- golang-github-blang-semver ~ 3.6.1-1~bpo10+1 (buster-backports).
- golang-github-flynn-json5 ~ 0.0+git20160717.7620272-2~bpo10+1 (to buster-backports).  
- golang-github-zyedidia-terminal ~ 0.0+git20180726.533c623-2~bpo10+1 (to buster-backports).  
- golang-github-go-errors-errors ~ 1.0.1-3~bpo10+1 (to buster-backports).  
- python-debianbts ~ 3.0.2~bpo10+1 (to buster-backports).  

#### Bug Fixes:

- #945232 for ruby-benchmark-suite.  
- #946904 for ruby-excon (CVE-2019-19779).  

#### Reviews and Sponsored Uploads:

- phpmyadmin for William Desportes.  

##### Miscellaneous:

- Outreachy mentoring for GitLab project for Sakshi Sangwan.  
- Raised various MRs upstream to sync Debian's package version with GitLab's upstream.  

---

One exciting blog post coming very soon.  

Until next time.  
`:wq` for today.
