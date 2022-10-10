+++
date = "2020-03-30"
title = "FOSS Activites in March 2020"
slug = "foss-in-march-20"
tags = [
    "debian",
    "monthly",
]
categories = [
    "debian",
    "open-source",
]
+++

Here's my (sixth) monthly update about the activities I've done in Debian this March.

## Debian LTS

This was my sixth month as a Debian LTS paid contributor.  
I was assigned 24.00 hours and worked on the following things:  

#### CVE Fixes and Announcements:

- Issued DLA 2131-1, fixing CVE-2014-6262, for rrdtool.  
  For Debian 8 "Jessie", this problem has been fixed in version 1.4.8-1.2+deb8u1.  

- Issued DLA 2131-2, fixing regression caused by DLA 2131-1, for rrdtool.  
  For Debian 8 "Jessie", this problem has been fixed in version 1.4.8-1.2+deb8u2.  

- Issued DLA 2135-1, fixing CVE-2020-9546, CVE-2020-9547, and CVE-2020-9548,  
  for jackson-databind.  
  For Debian 8 "Jessie", these problems have been fixed in version 2.4.2-2+deb8u12.  

- Issued DLA 2137-1, fixing CVE-2020-10232, for sleuthkit.  
  For Debian 8 "Jessie", this problem has been fixed in version 4.1.3-4+deb8u2.  

- Issued DLA 2139-1, fixing CVE-2020-5258 and CVE-2020-5259, for dojo.  
  For Debian 8 "Jessie", these problems have been fixed in version 1.10.2+dfsg-1+deb8u3.  

- Issued DLA 2141-1, fixing CVE-2020-10184 and CVE-2020-10185, for yubikey-val.  
  For Debian 8 "Jessie", these problems have been fixed in version 2.27-1+deb8u1.  

- Issued DLA 2146-1, fixing CVE-2019-15690, for libvncserver.  
  For Debian 8 "Jessie", this problem has been fixed in version 0.9.9+dfsg2-6.1+deb8u7.  

- Issued DLA 2147-1, fixing CVE-2019-17546, for gdal.  
  For Debian 8 "Jessie", this problem has been fixed in version 1.10.1+dfsg-8+deb8u2.  

- Issued DLA 2149-1, fixing CVE-2020-5267, for rails.  
  For Debian 8 "Jessie", this problem has been fixed in version 2:4.1.8-1+deb8u6.  

- Issued DLA 2153-1, fixing CVE-2020-10672 and CVE-2020-10673, for jackson-databind.  
  For Debian 8 "Jessie", these problems have been fixed in version 2.4.2-2+deb8u13.  

- Issued DLA 2154-1, fixing CVE-2020-10802 and CVE-2020-10803, for phpmyadmin.  
  For Debian 8 "Jessie", these problems have been fixed in version 4:4.2.12-2+deb8u9.  


#### Other LTS Work:

- Triaged [rrdtool](https://tracker.debian.org/pkg/rrdtool),
[sleuthkit](https://tracker.debian.org/pkg/sleuthkit),
[libarchive](https://tracker.debian.org/pkg/libarchive),
[dojo](https://tracker.debian.org/pkg/dojo),
[nethack](https://tracker.debian.org/pkg/nethack),
[libvncserver](https://tracker.debian.org/pkg/libvncserver),
[rails](https://tracker.debian.org/pkg/rails),
[jackson-databind](https://tracker.debian.org/pkg/jackson-databind),  
and [phpmyadmin](https://tracker.debian.org/pkg/phpmyadmin).  

- Traiged CVE-2019-20509/libarchive and marked it as not-affected for Jessie, Stretch, and Buster.  

---

## Debian Work

#### Uploads to the Archive:

- micro (2.0.2-1~bpo10+1) to buster-backports.  
- rails (2:5.2.4.1+dfsg-1) to unstable.  
- ruby-rack (2.0.8-1) to unstable.  
- ruby-grape (1.3.0-1) to experimental.  
- libgit2 (0.28.4+dfsg.1-3) to unstable.  
- micro (2.0.2-2) to unstable.  
- ruby-octokit (4.17.0-1) to unstable.  
- ruby-power-assert (1.1.6-1) to unstable.  
- rails (2:5.2.4.1+dfsg-2) to unstable.  
- ruby-octokit (4.17.0-2) to unstable.  
- ruby-method-source (1.0.0-1) to unstable.  
- libwebservice-ils-perl (0.18-1) to unstable.  
- libdata-hal-perl (1.001-1) to unstable.  
- rails (2:4.2.7.1-1+deb9u2) to stretch.  
- rails (2:5.2.2.1+dfsg-1+deb10u1) to buster.  
- libgit2 (0.28.4+dfsg.1-4) to unstable.  
- ruby-grape (1.3.1+git20200320.c8fd21b-1) to experimental.  
- ruby-grape-logging (1.8.3-1) to unstable.  
- ruby-grape (1.3.1+git20200320.c8fd21b-2) to unstable.  
- ruby-dry-equalizer (0.3.0-2) to unstable.  
- ruby-dry-core (0.4.9-2) to unstable.  
- ruby-dry-logic (1.0.5-2) to unstable.  
- ruby-dry-inflector (0.2.0-2) to unstable.  
- ruby-dry-container (0.7.2-2) to unstable.  
- ruby-dry-configurable (0.9.0-2) to unstable.  
- ruby-dry-types (1.2.2-2) to unstable.  
- micro (2.0.2-2~bpo10+1) to buster-backports.  
- golang-vbom-util (0.0~git20180919.efcd4e0-2) to unstable.  
- golang-github-tonistiigi-units (0.0~git20180711.6950e57-2) to unstable.  
- golang-github-jaguilar-vt100 (0.0~git20150826.2703a27-2) to unstable.  
- golang-github-grpc-ecosystem-grpc-opentracing (0.0~git20180507.8e809c8-2) to unstable.  
- rails (2:6.0.2.1+dfsg-3) to experimental.  
- libgit2 (0.99.0+dfsg.1-1) to experimental.  
- golang-github-goji-param (0.0~git20160927.d7f49fd-5) to unstable.  
- phpmyadmin-sql-parser (4.6.1-2) to unstable.  
- mariadb-mysql-kbs (1.2.10-2) to unstable.  
- golang-github-aleksi-pointer (1.1.0-1) to unstable.  
- golang-github-andreyvit-diff (0.0~git20170406.c7f18ee-2) to unstable.  
- golang-github-audriusbutkevicius-go-nat-pmp (0.0~git20160522.452c976-2) to unstable.  
- ruby-power-assert (1.1.7-1) to unstable.  
- ruby-test-unit (3.3.5-1) to unstable.  
- ruby-omniauth (1.9.1-1) to unstable.  
- ruby-warden (1.2.8-1) to unstable.  
- python-libais (0.17+git.20190917.master.e464cf8-2) to unstable.  
- lolcat (100.0.1-3) to unstable.  
- ruby-vips (2.0.17-1) to unstable.  

#### Bug Fixes:

- #836206 for lolcat.  
- #940338 for golang-github-audriusbutkevicius-go-nat-pmp.  
- #940335 for golang-github-andreyvit-diff.  
- #940334 for golang-github-aleksi-pointer.  
- #940362 for golang-github-goji-param.  
- #952025 for ruby-grape.  
- #867027 for ruby-grape.  
- #954529 for libgit2.  
- #954304 for rails (CVE-2020-5267) -- buster-pu.  
- #954304 for rails (CVE-2020-5267) -- stretch-pu.  
- #954304 for rails (CVE-2020-5267) -- unstable.  
- #953400 for micro.  
- #927889 for libgit2.  
- #952111 for micro.  

### Miscellaneous:  

- Sponsored a lot of uploads :)  
- Outreachy mentoring for GitLab project for Sakshi Sangwan.  
- Opened PRs & MRs upstream.  

---

Until next time.  
`:wq` for today.
