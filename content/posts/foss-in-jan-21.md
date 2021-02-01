+++
date = "2021-02-01 14:00:00 +0530"
title = "FOSS Activites in January 2021"
slug = "foss-in-jan-21"
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

Here's my (sixteenth) monthly update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 25th month of contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March 2019 and a [DD](https://wiki.debian.org/DebianDeveloper) on Christmas '19! \o/

This month was bat-shit crazy. Why? We'll come to it later, probably 15th of this month?  
Anyway, besides being crazy, hectic, adventerous, and the first of 2021, this month I was super-insanely busy. With what? Hm, more about this later this month! ^_^  

However, I still did some Debian stuff here and there. Here are the following things I worked on:

#### Uploads and bug fixes:

- [ruby-rack](https://tracker.debian.org/pkg/ruby-rack) (2.1.1-6) - Fixing [CVE-2020-8184](https://security-tracker.debian.org/tracker/CVE-2020-8184)/[bug #963477](https://bugs.debian.org/963477).
- [ruby-faye-websocket](https://tracker.debian.org/pkg/ruby-faye-websocket) (0.11.0-1) - Fixing [CVE-2020-15133](https://security-tracker.debian.org/tracker/CVE-2020-15133)/[bug #967061](https://bugs.debian.org/967061).
- [ruby-faye](https://tracker.debian.org/pkg/ruby-faye) (1.4.0-1) - Fixing [CVE-2020-11020](https://security-tracker.debian.org/tracker/CVE-2020-11020)/[bug #959392](https://bugs.debian.org/959392) and [CVE-2020-15134](https://security-tracker.debian.org/tracker/CVE-2020-15134)/[bug #967063](https://bugs.debian.org/967063).
- [ruby-rack](https://tracker.debian.org/pkg/ruby-rack) (2.1.4-2) - Fix failing tests and new upstream version, v2.1.4.
- [ruby-rake-ant](https://tracker.debian.org/pkg/ruby-rake-ant) (1.0.4-1) - Initial release, [bug #979498](https://bugs.debian.org/979498).
- [libgit2](https://tracker.debian.org/pkg/libgit2) (1.1.0+dfsg.1-4) - Source-only upload for migration.
- [ruby-scanf](https://tracker.debian.org/pkg/ruby-scanf) (1.0.0-1) - Initial release, [bug #979497](https://bugs.debian.org/979497).
- [polybar](https://tracker.debian.org/pkg/polybar) (3.5.4-1) - New upstream version, v3.5.4.
- [fpc](https://tracker.debian.org/pkg/fpc) (3.2.0+dfsg-10) - Severe crash fix for bugs [#979850](https://bugs.debian.org/979850), [#979853](https://bugs.debian.org/979853), [#979862](https://bugs.debian.org/979862), and [#979851](979851).
- [ruby-em-redis](https://tracker.debian.org/pkg/ruby-em-redis) (0.3.0+gh-3) - Fixing FTBFS, [bug #978975](https://bugs.debian.org/978975), as requested by Holger! :)
- [gdebi](https://tracker.debian.org/pkg/gdebi) (0.9.5.7+nmu4) - Fixing FTBFS, [bug #951923](https://bugs.debian.org/951923), as requested by Holger! :)
- [ruby-redcarpet](https://tracker.debian.org/pkg/ruby-redcarpet) (3.4.0-4+deb10u1) - Fixing [CVE-2020-26298](https://security-tracker.debian.org/tracker/CVE-2020-26298)/[bug #980057](https://bugs.debian.org/980057).
- [ruby-in-parallel](https://tracker.debian.org/pkg/ruby-in-parallel) (0.1.17-1.2) - Fixing autopkgtest, [bug #979700](https://bugs.debian.org/979700).
- [ruby-in-parallel](https://tracker.debian.org/pkg/ruby-in-parallel) (0.1.17-1.3) - Fixing random test failures, [bug #980585](https://bugs.debian.org/980585).
- [python-bottle](https://tracker.debian.org/pkg/python-bottle) (0.12.15-2+deb10u1) - Fixing [CVE-2020-28473](https://security-tracker.debian.org/tracker/CVE-2020-28473).

#### Other $things:

- Attended the Debian Ruby team meeting.
- Mentoring for newcomers.
- Moderation of -project mailing list.
- Sponsored `golang-github-gorilla-css` for Fedrico.

---

## Debian (E)LTS
{{< figure src="/images/debian-lts-small.png" >}}

[Debian Long Term Support (LTS)](https://www.freexian.com/en/services/debian-lts.html) is a project to extend the lifetime of all Debian stable releases to (at least) 5 years. Debian LTS is not handled by the Debian security team, but by a separate group of volunteers and companies interested in making it a success.  

And [Debian Extended LTS (ELTS)](https://deb.freexian.com/extended-lts) is its sister project, extending support to the Jessie release (+2 years after LTS support).

This was my sixteenth month as a Debian LTS and seventh month as a Debian ELTS paid contributor.  
I was assigned 26.00 hours for LTS and 36.75 hours for ELTS and worked on the following things:  

#### LTS CVE Fixes and Announcements:

- Issued [DLA 2518-1](https://lists.debian.org/debian-lts-announce/2021/01/msg00006.html), fixing [CVE-2020-35492](https://security-tracker.debian.org/tracker/CVE-2020-35492), for [cairo](https://tracker.debian.org/pkg/cairo).  
  For Debian 9 Stretch, these problems have been fixed in version 1.14.8-1+deb9u1.
- Issued [DLA 2525-1](https://lists.debian.org/debian-lts-announce/2021/01/msg00013.html), fixing [CVE-2018-19840](https://security-tracker.debian.org/tracker/CVE-2018-19840), [CVE-2018-19841](https://security-tracker.debian.org/tracker/CVE-2018-19841), [CVE-2019-11498](https://security-tracker.debian.org/tracker/CVE-2019-11498), [CVE-2019-1010315](https://security-tracker.debian.org/tracker/CVE-2019-1010315), [CVE-2019-1010317](https://security-tracker.debian.org/tracker/CVE-2019-1010317), [CVE-2019-1010319](https://security-tracker.debian.org/tracker/CVE-2019-1010319), and [CVE-2020-35738](https://security-tracker.debian.org/tracker/CVE-2020-35738), for [wavpack](https://tracker.debian.org/pkg/wavpack).  
  For Debian 9 Stretch, these problems have been fixed in version 5.0.0-2+deb9u3.
- Issued [DLA 2526-1](https://lists.debian.org/debian-lts-announce/2021/01/msg00014.html), fixing [CVE-2020-26298](https://security-tracker.debian.org/tracker/CVE-2020-26298), for [ruby-redcarpet](https://tracker.debian.org/pkg/ruby-redcarpet).  
  For Debian 9 Stretch, these problems have been fixed in version 3.3.4-2+deb9u1.
- Prepared [DSA 4831-1](https://lists.debian.org/debian-security-announce/2021/msg00010.html), fixing [CVE-2020-26298](https://security-tracker.debian.org/tracker/CVE-2020-26298), for [ruby-redcarpet](https://tracker.debian.org/pkg/ruby-redcarpet).
  For Debian 10 Buster, these problems have been fixed in version 3.4.0-4+deb10u1. The announcement was released by the Security Team.
- Issued [DLA 2528-1](https://lists.debian.org/debian-lts-announce/2021/01/msg00016.html), fixing TEMP-0000000-FAEBC0, for [gst-plugins-bad1.0](https://tracker.debian.org/pkg/gst-plugins-bad1.0).  
  For Debian 9 Stretch, these problems have been fixed in version 1.10.4-1+deb9u1.
- Issued [DLA 2529-1](https://lists.debian.org/debian-lts-announce/2021/01/msg00017.html), fixing [CVE-2021-3181](https://security-tracker.debian.org/tracker/CVE-2021-3181), for [mutt](https://tracker.debian.org/pkg/mutt).  
  For Debian 9 Stretch, these problems have been fixed in version 1.7.2-1+deb9u5.
- Issued [DLA 2531-1](https://lists.debian.org/debian-lts-announce/2021/01/msg00019.html)), fixing [CVE-2020-28473](https://security-tracker.debian.org/tracker/CVE-2020-28473), for [python-bottle](https://tracker.debian.org/pkg/python-bottle).  
  For Debian 9 Stretch, these problems have been fixed in version 0.12.13-1+deb9u1.
- Released [buster-pu update](https://tracker.debian.org/news/1225804/accepted-python-bottle-01215-2deb10u1-source-all-into-proposed-updates-stable-new-proposed-updates/), fixing [CVE-2020-28473](https://security-tracker.debian.org/tracker/CVE-2020-28473), for [python-bottle](https://tracker.debian.org/pkg/python-bottle).
  For Debian 10 Buster, these problems have been fixed in version 0.12.15-2+deb10u1.

#### ELTS CVE Fixes and Announcements:

- Issued [ELA 344-1](https://deb.freexian.com/extended-lts/updates/ela-344-1-apt/), fixing [CVE-2020-27350](https://security-tracker.debian.org/tracker/CVE-2020-27350), for [apt](https://tracker.debian.org/pkg/apt).  
  For Debian 8 Jessie, these problems have been fixed in version 1.0.9.8.7.
- Issued [ELA 346-1](https://deb.freexian.com/extended-lts/updates/ela-346-1-wavpack/), fixing [CVE-2016-10169](https://security-tracker.debian.org/tracker/CVE-2016-10169), [CVE-2018-19840](https://security-tracker.debian.org/tracker/CVE-2018-19840), [CVE-2019-1010319](https://security-tracker.debian.org/tracker/CVE-2019-1010319), and [CVE-2020-35738](https://security-tracker.debian.org/tracker/CVE-2020-35738), for [wavpack](https://tracker.debian.org/pkg/wavpack).  
  For Debian 8 Jessie, these problems have been fixed in version 4.70.0-1+deb8u1.
- Issued [ELA 347-1](https://deb.freexian.com/extended-lts/updates/ela-347-1-ruby-redcarpet/), fixing [CVE-2020-26298](https://security-tracker.debian.org/tracker/CVE-2020-26298), for [ruby-redcarpet](https://tracker.debian.org/pkg/ruby-redcarpet).  
  For Debian 8 Jessie, these problems have been fixed in version 3.1.2-1+deb8u1.
- Issued [ELA 348-1](https://deb.freexian.com/extended-lts/updates/ela-348-1-gst-plugins-bad1.0/), fixing TEMP-0000000-FAEBC0, for [gst-plugins-bad1.0](https://tracker.debian.org/pkg/gst-plugins-bad1.0).  
  For Debian 8 Jessie, these problems have been fixed in version 1.4.4-2.1+deb8u3.
- Issued [ELA 349-1](https://deb.freexian.com/extended-lts/updates/ela-349-1-mutt/), fixing [CVE-2021-3181](https://security-tracker.debian.org/tracker/CVE-2021-3181), for [mutt](https://tracker.debian.org/pkg/mutt).  
  For Debian 8 Jessie, these problems have been fixed in version 1.5.23-3+deb8u5.
- Issued [ELA 350-1](https://deb.freexian.com/extended-lts/updates/ela-350-1-python-bottle/), fixing [CVE-2020-28473](https://security-tracker.debian.org/tracker/CVE-2020-28473), for [python-bottle](https://tracker.debian.org/pkg/python-bottle).

#### Other (E)LTS Work:

- Front-desk duty from 28-12 until 03-01 and from 25-01 until 31-01 for both LTS and ELTS.
- Triaged [dropbear](https://tracker.debian.org/pkg/dropbear),
[gst-plugins-bad1.0](https://tracker.debian.org/pkg/gst-plugins-bad1.0),
[phpmyadmin](https://tracker.debian.org/pkg/phpmyadmin),
[qemu](https://tracker.debian.org/pkg/qemu),
[firefox-esr](https://tracker.debian.org/pkg/firefox-esr),
[thunderbird](https://tracker.debian.org/pkg/thunderbird),
[openldap](https://tracker.debian.org/pkg/openldap),
[libdatetime-timezone-perl](https://tracker.debian.org/pkg/libdatetime-timezone-perl),
[tzdata](https://tracker.debian.org/pkg/tzdata),
[wavpack](https://tracker.debian.org/pkg/wavpack), and
[ruby-redcarpet](https://tracker.debian.org/pkg/ruby-redcarpet).
- Marked CVE-2019-12953/dropbear as postponed for jessie.
- Marked CVE-2019-12953/dropbear as postponed for stretch.
- Marked CVE-2018-19841/wavpack as not-affected for jessie.
- Marked CVE-2019-1010315/wavpack as not-affected for jessie.
- Marked CVE-2019-1010317/wavpack as not-affected for jessie.
- Marked CVE-2021-21252/phpmyadmin as no-dsa for stretch.
- Marked CVE-2021-20196/qemu as postponed for stretch.
- Marked CVE-2021-21252/phpmyadmin as no-dsa for jessie.
- Marked CVE-2021-20196/qemu as postponed for jessie.
- Marked CVE-2020-11947/qemu as postponed for jessie.
- Marked CVE-2021-3326/glibc as no-dsa for jessie.
- Marked CVE-2021-3326/glibc as no-dsa for stretch.
- Marked CVE-2020-35517/qemu as not-affected instead of postponed for jessie.
- Auto EOL'ed csync2, firefox-esr, linux, thunderbird, and xen for jessie.
- General discussion on LTS private and [public mailing list](https://lists.debian.org/debian-lts/2021/01/threads.html).

---

## Other $things! \o/

#### Bugs and Patches

Well, I did report some bugs and issues and also sent some patches:

- [Issue #44](https://github.com/jamesgeorge007/github-activity-readme/issues/44) for github-activity-readme, asking for a feature request to set custom committer's email address.
- [Issue #711](https://github.com/libgit2/git2go/issues/711) for git2go, reporting build failure for the library.
- [PR #89](https://github.com/toshimaru/rubocop-rails_config/pull/89) for rubocop-rails_config, bumping `RuboCop::Packaging` to v0.5.
- [Issue #36](https://github.com/utkarsh2102/rubocop-packaging/issues/36) for rubocop-packaging, asking to try out mutant :)
- [PR #212](https://github.com/cucumber/cucumber-ruby-core/pull/212) for cucumber-ruby-core, bumping `RuboCop::Packaging` to v0.5.
- [PR #213](https://github.com/cucumber/cucumber-ruby-core/pull/213) for cucumber-ruby-core, enabling `RuboCop::Packaging`.
- [Issue #19](https://github.com/amedrz/behance/issues/19) for behance, asking to relax constraints on `faraday` and `faraday_middleware`.
- [PR #37](https://github.com/utkarsh2102/rubocop-packaging/pull/37) for rubocop-packaging, enabling tests against ruby3.0! \o/
- [PR #489](https://github.com/cucumber/cucumber-rails/pull/489) for cucumber-rails, bumping `RuboCop::Packaging` to v0.5.
- [Issue #362](https://github.com/Nheko-Reborn/nheko/issues/362) for nheko, reporting a crash when opening the application.
- [PR #1282](https://github.com/paper-trail-gem/paper_trail/pull/1282) for paper_trail, adding `RuboCop::Packaging` amongst other used extensions.
- [Bug #978640](https://bugs.debian.org/978640) for nheko Debian package, reporting a crash, as a result of libfmt7 regression.

#### Misc and Fun

Besides squashing bugs and submitting patches, I did some other things as well!

- Participated in my first [Advent of Code](https://adventofcode.com/) event! :)  
  Whilst it was indeed fun, I didn't really complete it. No reason, really. But I'll definitely come back stronger next year, heh! :)  
  All the solutions thus far could be found [here](https://github.com/utkarsh2102/AdventOfCode/).
- Did a couple of reviews for some PRs and triaged some bugs here and there, meh.
- Also did some cloud debugging, not so fun if you ask me, but cool enough to make me want to do it again! ^_^
- Worked along with pollo, zigo, ehashman, rlb, et al for puppet and puppetserver in Debian. OMG, they're so lovely! <3
- Ordered some interesting books to read January onward. New year resolution? Meh, not really. Or maybe. But nah.
- Also did some interesting stuff this month but can't really talk about it now. Hopefully sooooon.

---

Until next time.  
`:wq` for today.
