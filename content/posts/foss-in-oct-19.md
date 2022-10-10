+++
date = "2019-10-30"
title = "FOSS Activites in October 2019"
slug = "foss-in-oct-19"
tags = [
    "debian",
    "monthly",
]
categories = [
    "debian",
    "open-source",
]
+++

Here's my (first) monthly update about the activities I've done in Debian this October.

## Debian LTS

This was my first month as a Debian LTS paid contributor.  
I was assigned 10 hours and worked on the following things:

#### CVE Fixes and Announcements:

- Issued [DLA 1948-1](https://lists.debian.org/debian-lts-announce/2019/10/msg00007.html), fixing CVE-2019-13574, for ruby-mini-magick.  
  Details here:
  >  In lib/mini_magick/image.rb in ruby-mini-magick, a fetched remote image filename could cause remote command execution because Image.open input is directly passed to Kernel#open, which accepts a pipe character followed by a command.  

  For Debian 8 "Jessie", this has been fixed in 3.8.1-1+deb8u1.

- Issued [DLA 1961-1](https://lists.debian.org/debian-lts-announce/2019/10/msg00029.html), fixing CVE-2019-14464, CVE-2019-14496, and CVE-2019-14497, for milkytracker.  
  Details here:
  > XMFile::read in XMFile.cpp in milkyplay in MilkyTracker had a heap-based buffer overflow.  
    LoaderXM::load in LoaderXM.cpp in milkyplay in MilkyTracker had a stack-based buffer overflow.  
    ModuleEditor::convertInstrument in tracker/ModuleEditor.cpp in MilkyTracker had a heap-based buffer overflow.  

  For Debian 8 "Jessie", this has been fixed in 0.90.85+dfsg-2.2+deb8u1.  
  Furthermore, sent a patch to the maintainer, James, for fixing the same in Bullseye, Sid. Commit [here](https://salsa.debian.org/multimedia-team/milkytracker/commit/124dd45d1b75d952a76cddf9de76bf7232bc1624). Fixed in 1.02.00+dfsg-2.  

- Issued [DLA 1962-1](https://lists.debian.org/debian-lts-announce/2019/10/msg00030.html), fixing CVE-2017-18638, for graphite-web.  
  Details here:
  > The "send_email" function in graphite-web/webapp/graphite/composer/views.py in Graphite is vulnerable to SSRF. The vulnerable SSRF endpoint can be used by an attacker to have the Graphite web server request any resource. The response to this SSRF request is encoded into an image file and then sent to an e-mail address that can be supplied by the attacker. Thus, an attacker can exfiltrate any information.

  For Debian 8 "Jessie", this has been fixed in 0.9.12+debian-6+deb8u1.  
  Furthermore, sent a patch to the maintainer, Zigo, for fixing the same in Bullseye, Sid. Commit [here](https://salsa.debian.org/debian-graphite-team/graphite-web/commit/7e9ebc4f87966fdf35b2a87a6f3846acaab3e36b). Fixed in 1.1.4-5.  
  Also, sent a patch to the Security Team for fixing the same in Buster, but uploaded by Zigo himself. Commit [here](https://salsa.debian.org/debian-graphite-team/graphite-web/commit/3937fcf96ffd656ea85bb2ed15fe2b2ec6fb1712). Fixed in 1.1.4-3+deb10u1.

#### Miscellaneous:

- **Actually** fix CVE-2019-11027 upstream for ruby-openid. Pull request [here](https://github.com/openid/ruby-openid/pull/126).  
  Whilst this has been merged and released as v2.9.2, there are other login problems, as reported [here](https://github.com/openid/ruby-openid/issues/125).  

- Discuss with LTS Team Members about best practices for CVE-2019-11027 for ruby-openid's actual fix. Thread [here](https://lists.debian.org/debian-lts/2019/10/msg00091.html).  

- Triage Ansible for CVE-2019-14846 (which seems to be an easy fix) and CVE-2019-14858 (this kinda looks unaffected for Jessie, but not sure yet).

---

## Debian Uploads

#### Uploads to the Archive:

- ruby-fog-aws ~ 3.5.2-1.  
- librole-tiny-perl ~  2.001001-1.  
- gitlab ~ 12.1.14-1 (to experimental).  
- libmail-box-perl ~ 3.008-1.  
- ruby-invisible-captcha ~ 0.12.2-1.  
- ruby-gnome ~ 3.4.0-1.  
- gitlab-shell ~ 9.3.0+dfsg-1 (to experimental).  
- gitlab-workhorse ~ 8.8.1+debian-1 (to experimental).  
- gitaly ~ 1.59.3+dfsg-1.  
- python-marshmallow-sqlalchemy ~ 0.19.0-1.  
- gitlab ~ 12.2.9-1 (to experimental).

#### Bug Fixes:

- #942125 for ruby-invisible-captcha.  
- #941795 for ruby-gnome.  
- #940352 for golang-github-davecgh-go-spew.  
- #942456 for python-flask-marshmallow.  
- Autopkgtest failure for python-flask-marshmallow.  
- CVE-2019-{18446 to 18463} for gitlab.

#### Reviews and Sponsored Uploads:

- node-d3-geo ~ 1.11.6-1 for Abhijith Sheheer.  
- d3-format ~ 1:1.4.1-2 for Samyak Jain.  
- Reviewed node-regex-cache for Abhijith Sheheer.  
- Reviewed node-ansi-align for Abhijith Sheheer.  
- Reviewed node-color-name for Priyanka Saggu.  
- Reviewed node-webpack for Priyanka Saggu.

#### Fasttrack Repo (fasttrack.debian.net):

- Uploaded and ACCEPTED gitlab.  
- Uploaded and ACCEPTED ruby-jwt for Nilesh Patra.  
- Uploaded and ACCEPTED ruby-gitlab-sidekiq-fetcher.  
- Uploaded and ACCEPTED ruby-fog-aws for Samyak Jain.

---

Until next time.  
`:wq` for today.
