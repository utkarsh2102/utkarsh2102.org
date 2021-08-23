+++
date = "2021-07-01 02:10:00 +0530"
title = "FOSS Activites in June 2021"
slug = "foss-in-june-21"
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

Here's my (twenty-first) monthly but brief update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 30th month of actively contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March 2019 and a [DD](https://wiki.debian.org/DebianDeveloper) on Christmas '19! \o/

However, this wasn't  really a good month for mental health. And so apparently lesser work but still more than nothing, heh. :D

As a side note, this month, I spent a lot of time on Clubhouse, the new social auido app, at least in India. (I am sure you'd have heard?) Anyway, I made some friends there; more on that later, maybe? (ik, I say that a lot, but ugh, I'll get to it!)

Anyway, I did the following stuff in Debian:


#### Uploads and bug fixes:

- [rails](https://tracker.debian.org/pkg/rails) (2:5.2.2.1+dfsg-1+deb10u3) - Fix for [CVE-2021-22885](https://security-tracker.debian.org/tracker/CVE-2021-22904)/[#988214](https://bugs.debian.org/988214), [CVE-2021-22904](https://security-tracker.debian.org/tracker/CVE-2021-22904)/[#988214](https://bugs.debian.org/988214), and [CVE-2021-22880](https://security-tracker.debian.org/tracker/CVE-2021-22880).
- [eterm](https://tracker.debian.org/pkg/eterm) (0.9.6-6.1) - Fix [CVE-2021-33477](https://security-tracker.debian.org/tracker/CVE-2021-33477)/[#989041](https://bugs.debian.org/989041) for Debian unstable, a.k.a. sid.
- [eterm](https://tracker.debian.org/pkg/eterm) (0.9.6-5+deb10u1) - Fix [CVE-2021-33477](https://security-tracker.debian.org/tracker/CVE-2021-33477)/[#989041](https://bugs.debian.org/989041) for Debian 10, buster.
- [micro](https://tracker.debian.org/pkg/micro) (2.0.9-1) - New upstream version, v2.0.9.
- [ruby-httpclient](https://tracker.debian.org/pkg/ruby-httpclient) (2.8.3-3) - Disable tests related to `HTTP_PROXY` as Launchpad builders don't like them.

#### Other $things:

- Mentoring for newcomers.
- Moderation of -project mailing list.

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

This was my 5th month of actively contributing to [Ubuntu](https://ubuntu.com/about).
Now that I've joined [Canonical to work on Ubuntu full-time](https://utkarsh2102.com/posts/hello-canonical/), there's a bunch of things I do! \o/

This month, again, was dedicated to PHP 8.0, transitioning from PHP 7.4 to 8.0.
And finally, me and Bryce were able to complete the transition! \o/

This month, I also became an Ubuntu Core Developer. :D
I'll write about it in sometime; lol, yet another promise. Heh.

That said, the things that I mostly worked on are:

#### Uploads & Syncs:

- [2021-06-01] No-change rebuild for [php-email-validator/3.1.1-2build1](https://launchpad.net/ubuntu/+source/php-email-validator/3.1.1-2build1).
- [2021-06-01] [php-cache-integration-tests/0.17.0-1ubuntu1](https://launchpad.net/ubuntu/+source/php-cache-integration-tests/0.17.0-1ubuntu1) (fix build w/ symfony & php-twig.
- [2021-06-02] [php-league-mime-type-detection/1.5.1+ds-2ubuntu1](https://launchpad.net/ubuntu/+source/php-league-mime-type-detection/1.5.1+ds-2ubuntu1) (fix tests w/ PHP 8.0).
- [2021-06-02] [php-sabredav/1.8.12-9ubuntu1](https://launchpad.net/ubuntu/+source/php-sabredav/1.8.12-9ubuntu1) (fix autopkgtest w/ PHP 8.0).
- [2021-06-03] sync-request/php-doctrine-annotations (1.12.1-1) (from experimental) - [LP: #1929738](https://bugs.launchpad.net/ubuntu/+source/php-doctrine-annotations/+bug/1929738).
- [2021-06-03] [php-twig/3.3.2-1ubuntu2](https://launchpad.net/ubuntu/+source/php-twig/3.3.2-1ubuntu2) (make it build; circular-dependency breakthrough! \o/).
- [2021-06-03] [symfony/5.2.6+dfsg-1ubuntu1](https://launchpad.net/ubuntu/+source/symfony/5.2.6+dfsg-1ubuntu1/) (make it build; circular-dependency breakthrough! \o/).
- [2021-06-04] [php-cache-tag-interop/1.0.1-1ubuntu1](https://launchpad.net/ubuntu/+source/php-cache-tag-interop/1.0.1-1ubuntu1) (fix FTBFS w/ Psr/Cache).
- [2021-06-04] [php-doctrine-bundle/2.2.3-1ubuntu1](https://launchpad.net/ubuntu/+source/php-doctrine-bundle/2.2.3-1ubuntu1) (make it build; circular-test-dependency breakthrough! \o/).
- [2021-06-07] [symfony/5.2.6+dfsg-1ubuntu2](https://launchpad.net/ubuntu/+source/symfony/5.2.6+dfsg-1ubuntu2) (fix FTBFS & tests w/ PHP 8 & Psr/Cache).
- [2021-06-09] No-change rebuild for [phpmyadmin/4:5.0.4+dfsg2-2ubuntu3](https://launchpad.net/ubuntu/+source/phpmyadmin/4:5.0.4+dfsg2-2ubuntu3).
- [2021-06-09] [php-twig/3.3.2-1ubuntu3](https://launchpad.net/ubuntu/+source/php-twig/3.3.2-1ubuntu3) (re-enable tests & re-add symfony-based extensions).
- [2021-06-11] No-change rebuild for [zeroc-ice/3.7.5-2build1](https://launchpad.net/ubuntu/+source/zeroc-ice/3.7.5-2build1).
- [2021-06-11] No-change rebuild for [php-uopz/6.1.2-4build2](https://launchpad.net/ubuntu/+source/php-uopz/6.1.2-4build2).
- [2021-06-17] [php-text-captcha/1.0.2-8ubuntu1](https://launchpad.net/ubuntu/+source/php-text-captcha/1.0.2-8ubuntu1) (fix FTBFS w/ PHP 8).
- [2021-06-17] [php-imagick/3.4.4+php8.0+3.4.4-2+deb11u2ubuntu1](https://launchpad.net/ubuntu/+source/php-imagick/3.4.4+php8.0+3.4.4-2+deb11u2ubuntu1) (fix FTBFS w/ PHP 8).
- [2021-06-18] sync'd/doctrine ([2.8.4+dfsg-1](https://launchpad.net/ubuntu/+source/doctrine/2.8.4+dfsg-1)) (from experimental).
- [2021-06-18] [php-symfony-security-acl/3.1.1-1ubuntu1](https://launchpad.net/ubuntu/+source/php-symfony-security-acl/3.1.1-1ubuntu1) (fix FTBFS w/ PHP 8).
- [2021-06-19] [phpmyadmin/4:5.0.4+dfsg2-2ubuntu5](https://launchpad.net/ubuntu/+source/phpmyadmin/4:5.0.4+dfsg2-2ubuntu5) (fix uninstallability issues for php-defaults).
- [2021-06-19] [php-zend-stdlib/3.3.1-3ubuntu1](https://launchpad.net/ubuntu/+source/php-zend-stdlib/3.3.1-3ubuntu1) (fix tests w/ PHP 8).
- [2021-06-21] [phpseclib/1.0.19-3ubuntu2](https://launchpad.net/ubuntu/+source/phpseclib/1.0.19-3ubuntu2) (fix build & tests w/ PHP 8).
- [2021-06-22] filed hints w/ Iain (laney) to make php-defaults migrate - [MP #404519](https://code.launchpad.net/~utkarsh/britney/+git/britney/+merge/404519).
- [2021-06-23] announced the end of PHP 8.0's successful tranisition on ubuntu-devel@. Thread [here](https://lists.ubuntu.com/archives/ubuntu-devel/2021-June/041519.html)! \o/

#### +1 Maintenance:

- Shadowed Christian Ehrhardt on his +1. My report [here](https://lists.ubuntu.com/archives/ubuntu-devel/2021-June/041512.html).
  - Added hints for schleuder; [MP #404025](https://code.launchpad.net/~utkarsh/britney/+git/britney/+merge/404025).
  - Fixed [ruby-httpclient via 2.8.3-3](https://tracker.debian.org/news/1242716/accepted-ruby-httpclient-283-3-source-into-unstable/) in Debian.
  - Requested removal of ruby-gitlab-pg-query from Impish (-proposed) - [LP: #1931257](https://bugs.launchpad.net/ubuntu/+source/ruby-gitlab-pg-query/+bug/1931257).
  - Re-triggered python-django-debug-toolbar/1:3.2.1-1 for amd64 and it passed & migrated.
  - Fixed [ruby-rails-html-sanitizer via 1.3.0-2](https://tracker.debian.org/news/1242685/accepted-ruby-rails-html-sanitizer-130-2-source-into-unstable/) in Debian to make it work with newer API of ruby-loofah.
  - Re-triggered ruby-stackprof with glibc as triggers on amd64; it passed & unblocked glibc.
  - Re-triggered ruby-ferret with glibc as triggers on amd64; it passed & unblocked glibc.
  - Re-triggered ruby-hiredis with glibc as triggers on armhf; it passed & unblocked glibc.
  - Added hints for ruby-excon on s390x; [MP #404113](https://code.launchpad.net/~utkarsh/britney/+git/britney/+merge/404113).


#### Seed Operations:

- [2021-06-01] MP #403562/prips for Impish - [MP: #403562](https://code.launchpad.net/~utkarsh/ubuntu-seeds/+git/ubuntu-seeds/+merge/403562).
  - [2021-06-02] MP #403602/prips for Hirsute - [MP: #403602](https://code.launchpad.net/~utkarsh/ubuntu-seeds/+git/ubuntu-seeds/+merge/403602).
  - [2021-06-02] MP #403603/prips for Groovy - [MP: #403603](https://code.launchpad.net/~utkarsh/ubuntu-seeds/+git/ubuntu-seeds/+merge/403603).
  - [2021-06-02] MP #403604/prips for Focal - [MP: #403604](https://code.launchpad.net/~utkarsh/ubuntu-seeds/+git/ubuntu-seeds/+merge/403604).
  - [2021-06-02] MP #403605/prips for Bionic - [MP: #403605](https://code.launchpad.net/~utkarsh/ubuntu-seeds/+git/ubuntu-seeds/+merge/403605).
- [2021-06-17] MP #404326/python-aws-requests-auth for Impish - [MP #404326](https://code.launchpad.net/~utkarsh/ubuntu-seeds/+git/ubuntu-seeds/+merge/404326).
  - [2021-06-22] MP #404489/python-aws-requests-auth for Hirsute - [MP #404489](https://code.launchpad.net/~utkarsh/ubuntu-seeds/+git/ubuntu-seeds/+merge/404489).
  - [2021-06-22] MP #404490/python-aws-requests-auth for Groovy - [MP #404490](https://code.launchpad.net/~utkarsh/ubuntu-seeds/+git/ubuntu-seeds/+merge/404490).
  - [2021-06-22] MP #404491/python-aws-requests-auth for Focal - [MP #404491](https://code.launchpad.net/~utkarsh/ubuntu-seeds/+git/ubuntu-seeds/+merge/404491).
  - [2021-06-22] MP #404492/python-aws-requests-auth for Bionic - [MP #404492](https://code.launchpad.net/~utkarsh/ubuntu-seeds/+git/ubuntu-seeds/+merge/404492).


#### Bug Triages:

- [2021-06-04] [Friday bug triage](https://lists.ubuntu.com/archives/ubuntu-server/2021-June/008838.html).
- [2021-06-14] [Friday bug triage](https://lists.ubuntu.com/archives/ubuntu-server/2021-June/008849.html).
- [2021-06-18] [Friday bug triage](https://lists.ubuntu.com/archives/ubuntu-server/2021-June/008856.html).


---

## Debian (E)LTS
{{< figure src="/images/debian-lts-small.png" >}}

[Debian Long Term Support (LTS)](https://www.freexian.com/en/services/debian-lts.html) is a project to extend the lifetime of all Debian stable releases to (at least) 5 years. Debian LTS is not handled by the Debian security team, but by a separate group of volunteers and companies interested in making it a success.  

And [Debian Extended LTS (ELTS)](https://deb.freexian.com/extended-lts) is its sister project, extending support to the Jessie release (+2 years after LTS support).

This was my twentieth month as a Debian LTS and eleventh month as a Debian ELTS paid contributor.  
I was assigned 29.75 hours for LTS and 40.00 hours for ELTS and worked on the following things:  

#### LTS CVE Fixes and Announcements:

- Issued [DLA 2670-1](https://lists.debian.org/debian-lts-announce/2021/05/msg00025.html), fixing [CVE-2021-23017](https://security-tracker.debian.org/tracker/CVE-2021-23017), for [nginx](https://tracker.debian.org/pkg/nginx).  
  For Debian 9 stretch, these problems have been fixed in version 1.10.3-1+deb9u6.
- Issued [DLA 2671-1](https://lists.debian.org/debian-lts-announce/2021/05/msg00026.html), fixing [CVE-2021-33477](https://security-tracker.debian.org/tracker/CVE-2021-33477), for [rxvt-unicode](https://tracker.debian.org/pkg/rxvt-unicode).  
  For Debian 9 stretch, these problems have been fixed in version 9.22-1+deb9u1.
- Issued [DLA 2681-1](https://lists.debian.org/debian-lts-announce/2021/06/msg00010.html), fixing [CVE-2021-33477](https://security-tracker.debian.org/tracker/CVE-2021-33477), for [eterm](https://tracker.debian.org/pkg/eterm).  
  For Debian 9 stretch, these problems have been fixed in version 0.9.6-5+deb9u1.
- Prepped and uploaded a fix for [CVE-2021-33477](https://security-tracker.debian.org/tracker/CVE-2021-33477) to Debian unstable. News [here](https://tracker.debian.org/news/1242592/accepted-eterm-096-61-source-into-unstable/).  
  For Debian unstable, these problems have been fixed in version 0.9.6-6.1.
- Prepped and uploaded a fix for [CVE-2021-33477](https://security-tracker.debian.org/tracker/CVE-2021-33477) to Debian buster-pu. News [here](https://tracker.debian.org/news/1242616/accepted-eterm-096-5deb10u1-source-into-proposed-updates-stable-new-proposed-updates/).  
  For Debian 10 buster, these problems have been fixed in version 0.9.6-5+deb10u1.
- Issued [DLA 2682-1](https://lists.debian.org/debian-lts-announce/2021/06/msg00011.html), fixing [CVE-2021-33477](https://security-tracker.debian.org/tracker/CVE-2021-33477), for [mrxvt](https://tracker.debian.org/pkg/mrxvt).  
  For Debian 9 stretch, these problems have been fixed in version 0.5.4-2+deb9u1.
- Issued [DLA 2683-1](https://lists.debian.org/debian-lts-announce/2021/06/msg00012.html), fixing [CVE-2017-7483](https://security-tracker.debian.org/tracker/CVE-2017-7483) and [CVE-2021-33477](https://security-tracker.debian.org/tracker/CVE-2021-33477), for [rxvt](https://tracker.debian.org/pkg/rxvt).  
  For Debian 9 stretch, these problems have been fixed in version 1:2.7.10-7+deb9u2.
- Issued [DLA 2700-1](https://lists.debian.org/debian-lts-announce/2021/07/msg00000.html), fixing [CVE-2019-19630](https://security-tracker.debian.org/tracker/CVE-2019-19630), [CVE-2021-20308](https://security-tracker.debian.org/tracker/CVE-2021-20308), [CVE-2021-23158](https://security-tracker.debian.org/tracker/CVE-2021-23158), [CVE-2021-23165](https://security-tracker.debian.org/tracker/CVE-2021-23165), [CVE-2021-23180](https://security-tracker.debian.org/tracker/CVE-2021-23180), [CVE-2021-23191](https://security-tracker.debian.org/tracker/CVE-2021-23191), [CVE-2021-23206](https://security-tracker.debian.org/tracker/CVE-2021-23206), [CVE-2021-26252](https://security-tracker.debian.org/tracker/CVE-2021-26252), [CVE-2021-26259](https://security-tracker.debian.org/tracker/CVE-2021-26259), and [CVE-2021-26948](https://security-tracker.debian.org/tracker/CVE-2021-26948), for [htmldoc](https://tracker.debian.org/pkg/htmldoc).  
  For Debian 9 stretch, these problems have been fixed in version 1.8.27-8+deb9u1.

#### ELTS CVE Fixes and Announcements:

- Issued [ELA 437-1](https://deb.freexian.com/extended-lts/updates/ela-437-1-nginx/), fixing [CVE-2021-23017](https://security-tracker.debian.org/tracker/CVE-2021-23017), for [nginx](https://tracker.debian.org/pkg/nginx).  
  For Debian 8 jessie, these problems have been fixed in version 1.6.2-5+deb8u8.
- Issued [ELA 448-1](https://deb.freexian.com/extended-lts/updates/ela-448-1-cloud-int/), fixing [CVE-2021-3429](https://security-tracker.debian.org/tracker/CVE-2021-3429), for [cloud-int](https://tracker.debian.org/pkg/cloud-int).  
  For Debian 8 jessie, these problems have been fixed in version 0.7.6~bzr976-2+deb8u3.
- Issued [ELA 451-1](https://deb.freexian.com/extended-lts/updates/ela-451-1-htmldoc/), fixing [CVE-2021-20308](https://security-tracker.debian.org/tracker/CVE-2021-20308), [CVE-2021-23158](https://security-tracker.debian.org/tracker/CVE-2021-23158), [CVE-2021-23165](https://security-tracker.debian.org/tracker/CVE-2021-23165), [CVE-2021-23180](https://security-tracker.debian.org/tracker/CVE-2021-23180), [CVE-2021-23191](https://security-tracker.debian.org/tracker/CVE-2021-23191), [CVE-2021-23206](https://security-tracker.debian.org/tracker/CVE-2021-23206), [CVE-2021-26252](https://security-tracker.debian.org/tracker/CVE-2021-26252), [CVE-2021-26259](https://security-tracker.debian.org/tracker/CVE-2021-26259), and [CVE-2021-26948](https://security-tracker.debian.org/tracker/CVE-2021-26948), for [htmldoc](https://tracker.debian.org/pkg/htmldoc).  
  For Debian 8 jessie, these problems have been fixed in version 1.8.27-8+deb8u2.
- Issued [ELA 452-1](https://deb.freexian.com/extended-lts/updates/ela-452-1-python-pip/), fixing [CVE-2021-3572](https://security-tracker.debian.org/tracker/CVE-2021-3572), for [python-pip](https://tracker.debian.org/pkg/python-pip).  
  For Debian 8 jessie, these problems have been fixed in version 1.5.6-5+deb8u2.
- Issued [ELA 454-1](https://deb.freexian.com/extended-lts/updates/ela-454-1-djvulibre/), fixing [CVE-2021-3630](https://security-tracker.debian.org/tracker/CVE-2021-3630), for [djvulibre](https://tracker.debian.org/pkg/djvulibre).  
  For Debian 8 jessie, these problems have been fixed in version 3.5.25.4-4+deb8u4.
- Started working on intel-microcode fixes; have been waiting to see if there are any regressions noticed on sid, bullseye, and buster. Except for 0x906ea processors, everthing seems fine so far, at least.

#### Other (E)LTS Work:

- Front-desk duty from 28-06 until 04-07 for both LTS and ELTS.
- Triaged [rails](https://tracker.debian.org/pkg/rails),
[nginx](https://tracker.debian.org/pkg/nginx),
[eterm](https://tracker.debian.org/pkg/eterm),
[mrxvt](https://tracker.debian.org/pkg/mrxvt),
[rxvt](https://tracker.debian.org/pkg/rxvt),
[ieee-data](https://tracker.debian.org/pkg/ieee-data),
[cloud-init](https://tracker.debian.org/pkg/cloud-init),
[intel-microcode](https://tracker.debian.org/pkg/intel-microcode),
[htmldoc](https://tracker.debian.org/pkg/htmldoc),
[djvulibre](https://tracker.debian.org/pkg/djvulibre),
[composter](https://tracker.debian.org/pkg/composter), and
[curl](https://tracker.debian.org/pkg/curl).
- Mark CVE-2021-32563/thunar as no-dsa for stretch.
- Mark CVE-2017-7483 as fixed via +deb9u2 upload.
- Auto EOL'ed unrar-nonfree, darktable, mruby, htslib, ndpi, dcraw, libspring-security-2.0-java, rabbitmq-server, and linux for jessie.
- [LTS] Discussed ieee-data's fix for LTS. Thread [here](https://lists.debian.org/debian-lts/2021/06/msg00004.html).
- [ELTS] Discussed cloud-init's logs w/ Raphael and ask for a rebuild.
- [(E)LTS] Discussed intel-microcode's status w/ the maintainer and track regressions, et al.
- [(E)LTS] Discussed htmldoc's situation; about upgrade problems and prep a fix for that.
- Attended monthly Debian LTS meeting.
- Answered questions (& discussions) on IRC (#debian-lts and #debian-elts).
- General and other discussions on LTS private and [public mailing list](https://lists.debian.org/debian-lts/2021/06/threads.html).


---

Until next time.  
`:wq` for today.
