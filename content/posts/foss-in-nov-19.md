+++
date = "2019-12-01"
title = "FOSS Activites in November 2019"
slug = "foss-in-nov-19"
tags = [
    "debian",
    "monthly",
]
categories = [
    "debian",
    "open-source",
]
+++

Here's my (second) monthly update about the activities I've done in Debian this November.

## Debian LTS

This was my second month as a Debian LTS paid contributor.  
I was assigned 18 hours and worked on the following things:  

#### CVE Fixes and Announcements:

- Issued [DLA 1984-1](https://lists.debian.org/debian-lts-announce/2019/11/msg00005.html), fixing CVE-2019-17545, for gdal.  
  Details here:
  >  GDAL through 3.0.1 had a poolDestroy double free in OGRExpatRealloc in ogr/ogr_expat.cpp when the 10MB threshold was exceeded.  

  For Debian 8 "Jessie", this has been fixed in 1.10.1+dfsg-8+deb8u1.  
  Furthermore, sent a patch to the Security team for fixing the same in Stretch. Relevant .dsc can be found [here](https://mentors.debian.net/debian/pool/main/g/gdal/gdal_2.1.2+dfsg-5+deb9u1.dsc). Since I haven't heard back from the team yet, the upload to Stretch is still pending.  

- Issued [DLA 1986-1](https://lists.debian.org/debian-lts-announce/2019/11/msg00007.html), fixing CVE-2012017-1002201, for ruby-haml.  
  Details here:
  > In haml, when using user input to perform tasks on the server, characters like < > " ' must be escaped properly. In this case, the ' character was missed. An attacker can manipulate the input to introduce additional attributes, potentially executing code.  

  For Debian 8 "Jessie", this has been fixed in 4.0.5-2+deb8u1.  

- Issued [DLA 2004-1](https://lists.debian.org/debian-lts-announce/2019/11/msg00036.html), fixing CVE-2019-14824, for 389-ds-base.  
  Details here:
  > A flaw was found in the 'deref' plugin of 389-ds-base where it could use the 'search' permission to display attribute values. In some configurations, this could allow an authenticated attacker to view private attributes, such as password hashes.  

  For Debian 8 "Jessie", this has been fixed in 1.3.3.5-4+deb8u7.  
  Furthermore, sent a patch to the maintainer, Timo, for fixing the same in Bullseye, Sid. And to the Security team for Stretch and Buster. The patch can be found [here](https://bugs.debian.org/cgi-bin/bugreport.cgi?bug=944150#10).  

- Issued [DLA 2005-1](https://lists.debian.org/debian-lts-announce/2019/11/msg00035.html), fixing CVE-2019-18849, for tnef.  
  Details here:
  > In tnef, an attacker may be able to write to the victim's .ssh/authorized_keys file via an e-mail message with a crafted winmail.dat application/ms-tnef attachment, because of a heap-based buffer over-read involving strdup.  

  For Debian 8 "Jessie", this has been fixed in 1.4.9-1+deb8u4.  
  Furthermore, sent a patch to the maintainer for fixing the same in Bullseye, Sid. And to the Security team for Stretch and Buster. The patch can be found [here](https://bugs.debian.org/cgi-bin/bugreport.cgi?bug=944851#12).  

#### Miscellaneous:

- Fixed CVE-2019-11027 for ruby-openid in unstable. News [here](https://tracker.debian.org/news/1078349/accepted-ruby-openid-292debian-1-source-into-unstable/). This is in reference with the [DLA 1956-1](https://lists.debian.org/debian-lts-announce/2019/10/msg00014.html), issued by Brian May.  

- Triage libexif, libjpeg-turbo, tnef, and ansible for Jessie.  

- Pinged upstream of libexif and 389-ds-base for relevant commits. Whilst 389-ds-base is now fixed, the maintainer of libexif is still working on the fix.  

- In midst of fixing CVE-2019-18978 for ruby-rack-cors and CVE-2019-2201 for libjpeg-turbo.  

---

## Debian Uploads

#### Uploads to the Archive:

- ruby-openid ~ 2.9.2debian-1 (to unstable).  
- gitlab ~ 12.2.9-2 (to experimental).  
- node-yarnpkg ~ 1.19.1-1~bpo10+1 (to backports).  
- node-js-yaml ~ 3.13.1+dfsg-2~bpo10+1 (to backports).  
- ruby-sshkey ~ 2.0.0-2~bpo10+1 (to backports).  
- ruby-bootstrap-form ~ 4.2.0-2~bpo10+1 (to backports).  

#### Bug Fixes:

- #944906 for gitlab.  
- #930388 for ruby-openid.  
- #945232 for ruby-benchmark-suite.  

#### Reviews and Sponsored Uploads:

- node-hawk ~ 7.1.2+dfsg-1 for Sakshi Sangwan.  
- node-loud-rejection ~ 2.2.0-1 for Sakshi Sangwan.  
- node-lazy-cache ~ 2.0.2-1 for Sakshi Sangwan.  

---

Until next time.  
`:wq` for today.
