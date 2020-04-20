+++
date = "2020-03-01"
title = "FOSS Activites in February 2020"
slug = "foss-in-feb-20"
tags = [
    "debian",
    "monthly",
]
categories = [
    "debian",
    "open-source",
]
+++

Here's my (fifth) monthly update about the activities I've done in Debian this February.

## Debian LTS

This was my fifth month as a Debian LTS paid contributor.  
I was assigned 20.00 hours and worked on the following things:  

#### CVE Fixes and Announcements:

- Issued [DLA 2095-1](https://lists.debian.org/debian-lts-announce/2020/02/msg00003.html), fixing CVE-2020-7040, for storebackup.  
  Details here:
  > storeBackup.pl in storeBackup through 3.5 relies on the /tmp/storeBackup.lock pathname, which allows symlink attacks that possibly lead to privilege escalation.  

  For Debian 8 "Jessie", this problem has been fixed in version 3.2.1-1+deb8u1.  
  Furthermore, sent the patch for the security update for Stretch and Buster to the maintainer.  

- Issued [DLA 2113-1](https://lists.debian.org/debian-lts-announce/2020/02/msg00021.html), fixing CVE-2020-8631 and CVE-2020-8632 for cloud-init.  
  Details here:
  > For CVE-2020-8631, in cloud-init, relies on Mersenne Twister for a random password,  which makes it easier for attackers to predict passwords, because rand_str in cloudinit/util.py calls the random.choice function.  

  > For CVE-2020-8632, in cloud-init, rand_user_password in cloudinit/config/cc_set_passwords.py has a small default pwlen value, which makes it easier for attackers to guess passwords.  

  For Debian 8 "Jessie", this problem has been fixed in version 0.7.6~bzr976-2+deb8u1.  

- Issued [DLA 2116-1](https://lists.debian.org/debian-lts-announce/2020/02/msg00023.html), fixing CVE-2015-9542, for libpam-radius-auth.  
  Details here:
  > A vulnerability was found in pam_radius: the password length check was done incorrectly in the add_password() function in pam_radius_auth.c, resulting in a stack based buffer overflow.  

  This could be used to crash (DoS) an application using the PAM stack for authentication.

  For Debian 8 "Jessie", this problem has been fixed in version 1.3.16-4.4+deb8u1.  

- Issued [DLA 2127-1](https://lists.debian.org/debian-lts-announce/2020/02/msg00033.html), fixing CVE-2019-10785, for dojo.  
  Details here:
  > dojox was vulnerable to Cross-site Scripting. This was due to dojox.xmpp.util.xmlEncode only encoding the first occurrence of each character, not all of them.  

  For Debian 8 "Jessie", this problem has been fixed in version 1.10.2+dfsg-1+deb8u2.  

- Whilst Dylan issued [DLA 2120-1](https://lists.debian.org/debian-lts-announce/2020/02/msg00026.html), fixing CVE-2020-8130, for rake, I, with the Ruby team hat on, fixed the same issue for Stretch and Buster via proposed-updates.  
  This CVE was fixed via 10.5.0-2+deb9u1 and 12.3.1-3+deb10u1 respectively.  

#### Other LTS Work:

- Triaged [cloud-init](https://tracker.debian.org/pkg/cloud-init),
[slirp](https://tracker.debian.org/pkg/slirp),
[libpam-radius-auth](https://tracker.debian.org/pkg/libpam-radius-auth),
[dojo](https://tracker.debian.org/pkg/dojo),
and [qemu](https://tracker.debian.org/pkg/qemu).  

- Triaged CVE-2020-1711 and CVE-2020-8608 with more precision and discussed the details with Ola.  

- Started working on rrdtool for CVE-2014-6262.  

---

## Debian Work

This was a great month! MiniDebCamp -> FOSDEM -> Ruby Sprints. Blog post soon :D  
In the month of February, I did a lot of Debian work.  

#### Uploads to the Archive:

- ruby-rbtrace ~ 0.4.11-1 to experimental.  
- ruby-optimist ~ 3.0.0-1 to unstable.  
- ruby-ffi ~ 1.12.2+dfsg-1 to experimental.  
- ruby-otr-activerecord ~ 1.4.1-1 to unstable.  
- ruby-msfrpc-client ~ 1.1.2-1 to unstable.  
- ruby-dataobjects-postgres ~ 0.10.17-1 to unstable.  
- ruby-json ~ 2.3.0+dfsg-1 to unstable.  
- ruby-gettext ~ 3.3.3-1 to experimental.  
- ruby-mobile-fu ~ 1.4.0+github-3 to unstable.  
- ruby-rbtrace ~ 0.4.11-2 to unstable.  
- ruby-gettext ~ 3.3.3-2 to unstable.  
- ruby-otr-activerecord ~ 1.4.1-2 to unstable.  
- ruby-dry-core ~ 0.4.9-1 to unstable.  
- ruby-power-assert ~ 1.1.5-1 to unstable.  
- ruby-dry-equalizer ~ 0.3.0-1 to unstable.  
- ruby-dry-logic ~ 1.0.5-1 to unstable.  
- ruby-dry-configurable ~ 0.9.0-1 to unstable.  
- ruby-dry-inflector ~ 0.2.0-1 to unstable.  
- ruby-dry-container ~ 0.7.2-1 to unstable.  
- ruby-dry-types ~ 1.2.2-1 to unstable.  
- ruby-backports ~ 3.16.0-1 to unstable.  
- bundler ~ 2.1.4-1 to unstable.  
- ruby-tty-platform ~ 0.3.0-2 to unstable.  
- ruby-geocoder ~ 1.5.1-2 to unstable.  
- ruby-geocoder ~ 1.5.1-3 to unstable.  
- golang-code.cloudfoundry-bytefmt ~ 0.0~git20190818.854d396-2 to unstable.  
- ruby-google-cloud-core ~ 1.2.0-2 to unstable.  
- ruby-google-cloud-env ~ 1.2.0-2 to unstable.  
- ruby-terrapin ~ 0.6.0-2 to unstable.  
- ruby-unidecode ~ 1.0.0-2 to unstable.  
- ruby-optimist ~ 3.0.0-2 to unstable.  
- micro ~ 2.0.0-1 to unstable.  
- golang-github-zyedidia-tcell ~ 0.0~git20200210.f7f063a-1 to unstable.  
- micro ~ 2.0.0-2 to unstable.  
- libgit2 ~ 0.28.4+dfsg.1-1 to experimental.  
- libgit2 ~ 0.28.4+dfsg.1-2 to unstable.  
- rails ~ 2:5.2.3+dfsg-3 to unstable.  
- chef ~ 13.8.7-5 to unstable.  
- chef ~ 13.8.7-6 to unstable.  
- ruby-apollo-upload-server ~ 2.0.0~beta3-2 to unstable.  
- ruby-strptime ~ 0.2.3-5 to unstable.  
- ruby-rugged ~ 0.28.4.1+ds-1 to unstable.  
- golang-gopkg-libgit2-git2go.v28 ~ 0.28.4-1 to unstable.  
- libpam-radius-auth ~ 1.4.0-3 to unstable.  
- ruby-octokit ~ 4.16.0-1 to unstable.  
- ruby-memory-profiler ~ 0.9.14-3 to unstable.  
- ruby-rails-assets-diaspora-jsxc ~ 0.1.5+dfsg2~develop.7-4 to unstable.  
- golang-github-zyedidia-tcell ~ 1.4.4-1 to unstable.  
- micro ~ 2.0.1-1 to unstable.  
- micro ~ 2.0.2-1 to unstable.  
- golang-github-zyedidia-tcell ~ 1.4.4-1~bpo10+1 to buster-backports.  
- golang-gopkg-libgit2-git2go.v28 ~ 0.28.5-1 to unstable.  
- rake ~ 12.3.1-3+deb10u1 to buster.  
- rake ~ 10.5.0-2+deb9u1 to stretch.  
- ruby-rbtrace ~ 0.4.11-1 to experimental.  
- ruby-optimist ~ 3.0.0-1 to unstable.  
- ruby-ffi ~ 1.12.2+dfsg-1 to experimental.  
- ruby-otr-activerecord ~ 1.4.1-1 to unstable.  
- ruby-msfrpc-client ~ 1.1.2-1 to unstable.  
- ruby-dataobjects-postgres ~ 0.10.17-1 to unstable.  
- ruby-json ~ 2.3.0+dfsg-1 to unstable.  
- ruby-gettext ~ 3.3.3-1 to experimental.  
- ruby-mobile-fu ~ 1.4.0+github-3 to unstable.  
- ruby-rbtrace ~ 0.4.11-2 to unstable.  
- ruby-gettext ~ 3.3.3-2 to unstable.  
- ruby-otr-activerecord ~ 1.4.1-2 to unstable.  
- ruby-dry-core ~ 0.4.9-1 to unstable.  
- ruby-power-assert ~ 1.1.5-1 to unstable.  
- ruby-dry-equalizer ~ 0.3.0-1 to unstable.  
- ruby-dry-logic ~ 1.0.5-1 to unstable.  
- ruby-dry-configurable ~ 0.9.0-1 to unstable.  
- ruby-dry-inflector ~ 0.2.0-1 to unstable.  
- ruby-dry-container ~ 0.7.2-1 to unstable.  
- ruby-dry-types ~ 1.2.2-1 to unstable.  
- ruby-backports ~ 3.16.0-1 to unstable.  
- bundler ~ 2.1.4-1 to unstable.  
- ruby-tty-platform ~ 0.3.0-2 to unstable.  
- ruby-geocoder ~ 1.5.1-2 to unstable.  
- ruby-geocoder ~ 1.5.1-3 to unstable.  
- golang-code.cloudfoundry-bytefmt ~ 0.0~git20190818.854d396-2 to unstable.  
- ruby-google-cloud-core ~ 1.2.0-2 to unstable.  
- ruby-google-cloud-env ~ 1.2.0-2 to unstable.  
- ruby-terrapin ~ 0.6.0-2 to unstable.  
- ruby-unidecode ~ 1.0.0-2 to unstable.  
- ruby-optimist ~ 3.0.0-2 to unstable.  
- micro ~ 2.0.0-1 to unstable.  
- golang-github-zyedidia-tcell ~ 0.0~git20200210.f7f063a-1 to unstable.  
- micro ~ 2.0.0-2 to unstable.  
- libgit2 ~ 0.28.4+dfsg.1-1 to experimental.  
- libgit2 ~ 0.28.4+dfsg.1-2 to unstable.  
- rails ~ 2:5.2.3+dfsg-3 to unstable.  
- chef ~ 13.8.7-5 to unstable.  
- chef ~ 13.8.7-6 to unstable.  
- ruby-apollo-upload-server ~ 2.0.0~beta3-2 to unstable.  
- ruby-strptime ~ 0.2.3-5 to unstable.  
- ruby-rugged ~ 0.28.4.1+ds-1 to unstable.  
- golang-gopkg-libgit2-git2go.v28 ~ 0.28.4-1 to unstable.  
- libpam-radius-auth ~ 1.4.0-3 to unstable.  
- ruby-octokit ~ 4.16.0-1 to unstable.  
- ruby-memory-profiler ~ 0.9.14-3 to unstable.  
- ruby-rails-assets-diaspora-jsxc ~ 0.1.5+dfsg2~develop.7-4 to unstable.  
- golang-github-zyedidia-tcell ~ 1.4.4-1 to unstable.  
- micro ~ 2.0.1-1 to unstable.  
- micro ~ 2.0.2-1 to unstable.  
- golang-github-zyedidia-tcell ~ 1.4.4-1~bpo10+1 to buster-backports.  
- golang-gopkg-libgit2-git2go.v28 ~ 0.28.5-1 to unstable.  
- rake ~ 12.3.1-3+deb10u1 to buster.  
- rake ~ 10.5.0-2+deb9u1 to stretch.  
- ruby-rbtrace ~ 0.4.11-1 to experimental.  
- ruby-optimist ~ 3.0.0-1 to unstable.  
- ruby-ffi ~ 1.12.2+dfsg-1 to experimental.  
- ruby-otr-activerecord ~ 1.4.1-1 to unstable.  
- ruby-msfrpc-client ~ 1.1.2-1 to unstable.  
- ruby-dataobjects-postgres ~ 0.10.17-1 to unstable.  
- ruby-json ~ 2.3.0+dfsg-1 to unstable.  
- ruby-gettext ~ 3.3.3-1 to experimental.  
- ruby-mobile-fu ~ 1.4.0+github-3 to unstable.  
- ruby-rbtrace ~ 0.4.11-2 to unstable.  
- ruby-gettext ~ 3.3.3-2 to unstable.  
- ruby-otr-activerecord ~ 1.4.1-2 to unstable.  
- ruby-dry-core ~ 0.4.9-1 to unstable.  
- ruby-power-assert ~ 1.1.5-1 to unstable.  
- ruby-dry-equalizer ~ 0.3.0-1 to unstable.  
- ruby-dry-logic ~ 1.0.5-1 to unstable.  
- ruby-dry-configurable ~ 0.9.0-1 to unstable.  
- ruby-dry-inflector ~ 0.2.0-1 to unstable.  
- ruby-dry-container ~ 0.7.2-1 to unstable.  
- ruby-dry-types ~ 1.2.2-1 to unstable.  
- ruby-backports ~ 3.16.0-1 to unstable.  
- bundler ~ 2.1.4-1 to unstable.  
- ruby-tty-platform ~ 0.3.0-2 to unstable.  
- ruby-geocoder ~ 1.5.1-2 to unstable.  
- ruby-geocoder ~ 1.5.1-3 to unstable.  
- golang-code.cloudfoundry-bytefmt ~ 0.0~git20190818.854d396-2 to unstable.  
- ruby-google-cloud-core ~ 1.2.0-2 to unstable.  
- ruby-google-cloud-env ~ 1.2.0-2 to unstable.  
- ruby-terrapin ~ 0.6.0-2 to unstable.  
- ruby-unidecode ~ 1.0.0-2 to unstable.  
- ruby-optimist ~ 3.0.0-2 to unstable.  
- micro ~ 2.0.0-1 to unstable.  
- golang-github-zyedidia-tcell ~ 0.0~git20200210.f7f063a-1 to unstable.  
- micro ~ 2.0.0-2 to unstable.  
- libgit2 ~ 0.28.4+dfsg.1-1 to experimental.  
- libgit2 ~ 0.28.4+dfsg.1-2 to unstable.  
- rails ~ 2:5.2.3+dfsg-3 to unstable.  
- chef ~ 13.8.7-5 to unstable.  
- chef ~ 13.8.7-6 to unstable.  
- ruby-apollo-upload-server ~ 2.0.0~beta3-2 to unstable.  
- ruby-strptime ~ 0.2.3-5 to unstable.  
- ruby-rugged ~ 0.28.4.1+ds-1 to unstable.  
- golang-gopkg-libgit2-git2go.v28 ~ 0.28.4-1 to unstable.  
- libpam-radius-auth ~ 1.4.0-3 to unstable.  
- ruby-octokit ~ 4.16.0-1 to unstable.  
- ruby-memory-profiler ~ 0.9.14-3 to unstable.  
- ruby-rails-assets-diaspora-jsxc ~ 0.1.5+dfsg2~develop.7-4 to unstable.  
- golang-github-zyedidia-tcell ~ 1.4.4-1 to unstable.  
- micro ~ 2.0.1-1 to unstable.  
- micro ~ 2.0.2-1 to unstable.  
- golang-github-zyedidia-tcell ~ 1.4.4-1~bpo10+1 to buster-backports.  
- golang-gopkg-libgit2-git2go.v28 ~ 0.28.5-1 to unstable.  
- rake ~ 12.3.1-3+deb10u1 to buster.  
- rake ~ 10.5.0-2+deb9u1 to stretch.  

#### Bug Fixes:

- #952283 for micro.  
- #951396 for libpam-radius-auth (CVE-2015-9542)).  
- #936866 for libgit2.  
- #913241 for libgit2.  
- #949870 for ruby-geocoder (CVE-2020-7981).  
- #842504 for bundler (CVE-2016-7954).  
- #945481 for bundler.  
- #950877 for ruby-dry-types.  
- #950870 for ruby-dry-container.  
- #950868 for ruby-dry-inflector.  
- #950867 for ruby-dry-configurable.  
- #950863 for ruby-dry-logic.  
- #950855 for ruby-dry-equalizer.  
- #950846 for ruby-dry-core.  
- #950656 for ruby-msfrpc-client.  
- #950651 for ruby-otr-activerecord.  
- #946423 for ruby-optimist.  

### Miscellaneous:  

- Sponsored lots of uploads :)  
- Outreachy mentoring for GitLab project for Sakshi Sangwan.  
- Ruby Sprint! \o/
- Opened PRs & MRs upstream.  

---

Until next time.  
`:wq` for today.
