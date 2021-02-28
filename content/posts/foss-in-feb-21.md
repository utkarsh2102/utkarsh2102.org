+++
date = "2021-03-01 16:00:00 +0530"
title = "FOSS Activites in February 2021"
slug = "foss-in-feb-21"
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

Here's my (seventeenth) monthly update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 26th month of active contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March 2019 and a [DD](https://wiki.debian.org/DebianDeveloper) on Christmas '19! \o/

This month was a nice mix of amusement, excitement, nervousness, and craziness. More on it below.  
Anyway, whilst I was super-insanely busy this month, I still did some Debian stuff here and there. Here are the following things I worked on:

#### Uploads and bug fixes:

- [ruby-mechanize](https://tracker.debian.org/pkg/ruby-mechanize) (2.7.7-1) - Fixing [CVE-2021-21289](https://security-tracker.debian.org/tracker/CVE-2021-21289).
- [rails](https://tracker.debian.org/pkg/rails) (2:6.0.3.4+dfsg-3) - Fixing silent build failure, [bug #979133](https://bugs.debian.org/979133).
- [tiledb](https://tracker.debian.org/pkg/tiledb) (1.7.7-1.1) - NMU + source-only upload for migration.
- [ruby-launchy](https://tracker.debian.org/pkg/ruby-launchy) (2.5.0-3) - Add Breaks+Replaces for launchy; fixing [bug #974046](https://bugs.debian.org/974046).
- [ruby-upr](https://tracker.debian.org/pkg/ruby-upr) (0.3.0-3) - Fixing FTBFS + autopkgtest; cf: [bug #883370](https://bugs.debian.org/883370).
- [gdisk](https://tracker.debian.org/pkg/gdisk) (1.0.6-1.1) - Add Restrictions: allow-stderr for autopkgtest; fixing [bug #981231](https://bugs.debian.org/981231).
- [test-check-clojure](https://tracker.debian.org/pkg/test-check-clojure) (0.9.0-4) - Fixing FTBFS + autpkgtest; cf: [bug #982721](https://bugs.debian.org/982721).
- [rails](https://tracker.debian.org/pkg/rails) (2:6.0.3.5+dfsg-1) - Fixing [CVE-2021-22880](https://security-tracker.debian.org/tracker/CVE-2021-22880) and [CVE-2021-22881](https://security-tracker.debian.org/tracker/CVE-2021-22881).
- [ruby-mechanize](https://tracker.debian.org/pkg/ruby-mechanize) (2.7.6-1+deb10u1) - pu-upload, fixing [CVE-2021-21289](https://security-tracker.debian.org/tracker/CVE-2021-21289).
- [ruby-handlebars-assets](https://tracker.debian.org/pkg/ruby-handlebars-assets) (2:0.23.8+dfsg-3) - Fixing autpkgtest by embedding a dummy rails app.
- [ruby-rails-assets-emojione](https://tracker.debian.org/pkg/ruby-rails-assets-emojione) (2.2.6-5) - Fixing autpkgtest by embedding a dummy rails app.
- [ruby-rails-assets-jquery-colorbox](https://tracker.debian.org/pkg/ruby-rails-assets-jquery-colorbox) (1.6.3~dfsg-7) - Fixing autpkgtest by embedding a dummy rails app.
- [ruby-rails-assets-jquery.slimscroll](https://tracker.debian.org/pkg/ruby-rails-assets-jquery.slimscroll) (1.3.6+dfsg-3) - Fixing autpkgtest by embedding a dummy rails app.
- [ruby-rails-assets-markdown-it](https://tracker.debian.org/pkg/ruby-rails-assets-markdown-it) (8.4.2-5) - Fixing autpkgtest by embedding a dummy rails app.
- [ruby-mousetrap-rails](https://tracker.debian.org/pkg/ruby-mousetrap-rails) (1.4.6-7) - Fixing autpkgtest by embedding a dummy rails app.
- [ruby-rails-assets-jquery-fullscreen-plugin](https://tracker.debian.org/pkg/ruby-rails-assets-jquery-fullscreen-plugin) (0.5.0+dfsg-4) - Fixing autpkgtest by embedding a dummy rails app.

#### Other $things:

- Attended the Debian LTS team meeting.
- Mentoring for newcomers.
- Moderation of -project mailing list.
- Sponsored `ruby-rspec-stubbed-env` for Cédric Boutillier, heh :P

---

## Debian (E)LTS
{{< figure src="/images/debian-lts-small.png" >}}

[Debian Long Term Support (LTS)](https://www.freexian.com/en/services/debian-lts.html) is a project to extend the lifetime of all Debian stable releases to (at least) 5 years. Debian LTS is not handled by the Debian security team, but by a separate group of volunteers and companies interested in making it a success.  

And [Debian Extended LTS (ELTS)](https://deb.freexian.com/extended-lts) is its sister project, extending support to the Jessie release (+2 years after LTS support).

This was my sixteenth month as a Debian LTS and seventh month as a Debian ELTS paid contributor.  
I was assigned 26.00 hours for LTS and 36.75 hours for ELTS and worked on the following things:  
(however, I worked extra for 9 hours for LTS and 9 hours for ELTS this month, which I intend to balance from the next month!)

#### LTS CVE Fixes and Announcements:

- Issued [DLA 2518-1](https://lists.debian.org/debian-lts-announce/2021/01/msg00006.html), fixing [CVE-2020-35492](https://security-tracker.debian.org/tracker/CVE-2020-35492), for [cairo](https://tracker.debian.org/pkg/cairo).  
  For Debian 9 Stretch, these problems have been fixed in version 1.14.8-1+deb9u1.
- Issued [DLA 2525-1](https://lists.debian.org/debian-lts-announce/2021/01/msg00013.html), fixing [CVE-2018-19840](https://security-tracker.debian.org/tracker/CVE-2018-19840), [CVE-2018-19841](https://security-tracker.debian.org/tracker/CVE-2018-19841), [CVE-2019-11498](https://security-tracker.debian.org/tracker/CVE-2019-11498), [CVE-2019-1010315](https://security-tracker.debian.org/tracker/CVE-2019-1010315), [CVE-2019-1010317](https://security-tracker.debian.org/tracker/CVE-2019-1010317), [CVE-2019-1010319](https://security-tracker.debian.org/tracker/CVE-2019-1010319), and [CVE-2020-35738](https://security-tracker.debian.org/tracker/CVE-2020-35738), for [wavpack](https://tracker.debian.org/pkg/wavpack).  
  For Debian 9 Stretch, these problems have been fixed in version 5.0.0-2+deb9u3.
- Issued [DLA 2526-1](https://lists.debian.org/debian-lts-announce/2021/01/msg00014.html), fixing [CVE-2020-26298](https://security-tracker.debian.org/tracker/CVE-2020-26298), for [ruby-redcarpet](https://tracker.debian.org/pkg/ruby-redcarpet).  
  For Debian 9 Stretch, these problems have been fixed in version 3.3.4-2+deb9u1.
- Prepared [DSA 4831-1](https://lists.debian.org/debian-security-announce/2021/msg00010.html), fixing [CVE-2020-26298](https://security-tracker.debian.org/tracker/CVE-2020-26298), for [ruby-redcarpet](https://tracker.debian.org/pkg/ruby-redcarpet).
  For Debian 10 Buster, these problems have been fixed in version 3.4.0-4+deb10u1. The announcement was released by the Security Team.
- Issued [DLA 2528-1](https://lists.debian.org/debian-lts-announce/2021/01/msg00016.html), fixing [CVE-2021-3185](https://security-tracker.debian.org/tracker/CVE-2021-3185), for [gst-plugins-bad1.0](https://tracker.debian.org/pkg/gst-plugins-bad1.0).  
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
- Issued [ELA 348-1](https://deb.freexian.com/extended-lts/updates/ela-348-1-gst-plugins-bad1.0/), fixing [CVE-2021-3185](https://security-tracker.debian.org/tracker/CVE-2021-3185), for [gst-plugins-bad1.0](https://tracker.debian.org/pkg/gst-plugins-bad1.0).  
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
[jasper](https://tracker.debian.org/pkg/jasper),
[ckeditor](https://tracker.debian.org/pkg/ckeditor),
[liblivemedia](https://tracker.debian.org/pkg/liblivemedia),
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
- Marked CVE-2021-2627{1,2}/ckeditor as postponed for jessie.
- Marked CVE-2020-24027/liblivemedia as no-dsa for stretch.
- Marked CVE-2021-2627{1,2}/ckeditor as postponed for stretch.
- Auto EOL'ed csync2, firefox-esr, linux, thunderbird, collabtive, activemq, and xen for jessie.
- Got my **first ever** CVE assigned - [CVE-2021-3181](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2021-3181) for mutt. Weeeehooooo! \o/
- Attended the monthly LTS meeting. Logs [here](http://meetbot.debian.net/debian-lts/2021/debian-lts.2021-01-28-14.58.html).
- General discussion on LTS private and [public mailing list](https://lists.debian.org/debian-lts/2021/01/threads.html).

---

## Interesting Bits!

- This January, on 23rd and 24th, we had [Mini DebConf India 2021 online](https://in2021.mini.debconf.org/).  
  I had a talk as well, titled, "[Why Point Releases are important and how you can help
  prepare them?](https://in2021.mini.debconf.org/talks/18-why-point-releases-are-important-and-how-you-can-help-prepare-them/)".

  It was a fun and a very short talk, where I just list out the reasons and ways to help in
  the preparation of "point releases". I did some experimentation with this talk, figuring
  out what works for the audience and what doesn't and where can I improve for the next time
  I talk about this topic! \o/  
  You can listen to the talk [here](https://ftp.acc.umu.se/pub/debian-meetings/2021/MiniDebConf-India/18-why-point-releases-are-important-and-how-you-can-help-prepare-them.webm)
  and let me know if you have any feedback!

  Anyway, the conference lasted for 2 days and I also did some volunteering (talk director,
  talk miester) in Hindi and English, both! It was all so fun and new. Anyway, here's the picture we took:
  ![](/images/minidebconf_india2021.png#center)

- In another exciting news, I got my first CVE assigned!!! \o/  
  No, it is not something that I found, it was discovered by Tavis Ormandy. I just assigned
  this a CVE ID, [CVE-2021-3181](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2021-3181).  
  This is my first, so I am very excited about this! ^_^

- Besides, there's something more that is in the pipelines. Can't talk about it now, shh. But
  hopefully very sooooooon!

---

## Other $things! \o/

This month was tiresome, with most of the time being spent on the Debian stuff, I did
very little work outside it, really. The issues and patches that I sent are:

- [Issue #700](https://github.com/vmg/redcarpet/issues/700) for redcarpet, asking for a reproducer for CVE-2020-26298 and some additional patch related queries.
- [Issue #7](https://github.com/samwoods1/in-parallel/issues/7) for in-parallel, asking them to not use relative paths for tests.
- [Issue #8](https://github.com/samwoods1/in-parallel/issues/8) for in-parallel, reporting a test failure for the library.
- [Issue #2](https://github.com/jruby/rake-ant/issues/2) for rake-ant, asking them to bump their dependencies to a newer version.
- [PR #3](https://github.com/jruby/rake-ant/pull/3) for rake-ant, bumping the dependencies to a newer version, fixing the above issue, heh.
- [Issue #4](https://github.com/jruby/rake-ant/issues/4) for rake-ant, requesting to drop `git` from their gemspec.
- [PR #5](https://github.com/jruby/rake-ant/pull/5) for rake-ant, dropping `git` from gemspec, fixing the above issue, heh.
- [Issue #95](https://github.com/dbry/WavPack/issues/95) for WavPack, asking for a review of past security vulnerabilites wrt v4.70.0.
- Reviewed [PR #128](https://github.com/openid/ruby-openid/pull/128) for ruby-openid, addressing the past regression with CVE fix merge.
- Reviewed [PR #63](https://github.com/CocoaPods/cocoapods-acknowledgements/pull/63) for cocoapods-acknowledgements, updating redcarpet to v3.5.1, as a safety measure due to recently discovered vulnerability.
- [Issue #1331](https://github.com/bottlepy/bottle/issues/1331) for bottle, asking for relevant commits for CVE-2020-28473 and clarifying other things.
- [Issue #5](https://github.com/libc/em-redis/issues/5) for em-redis, reporting test failures on IPv6-only build machines.
- [Issue #939](https://github.com/eventmachine/eventmachine/issues/939) for eventmachine, reporting test failures for em-redis on IPv6-only build machines.

---

Until next time.  
`:wq` for today.
