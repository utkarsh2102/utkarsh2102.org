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


---

Until next time.  
`:wq` for today.