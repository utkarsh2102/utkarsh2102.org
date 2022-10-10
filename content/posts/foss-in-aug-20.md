+++
date = "2020-08-30 21:30:00 +0530"
title = "FOSS Activites in August 2020"
slug = "foss-in-aug-20"
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
    "gsoc"
]
categories = [
    "debian",
    "open-source",
    "gsoc"
]
+++

Here's my (eleventh) monthly update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 20th month of contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March last year and a [DD](https://wiki.debian.org/DebianDeveloper) last Christmas! \o/

Well, this month we had [DebConf](https://debconf20.debconf.org/)! \o/  
(more about this later this week!)

Anyway, here are the following things I did in Debian this month:

#### Uploads and bug fixes:

- [rubocop](https://tracker.debian.org/pkg/rubocop) (0.89.1+dfsg-1) - New upstream version for `RuboCop::Packaging`.  
- [ruby-rubocop-ast](https://tracker.debian.org/pkg/ruby-rubocop-ast) (0.3.0+dfsg-1) - New upstream version for `RuboCop`'s latest version.  
- [ruby-rubocop-packaging](https://tracker.debian.org/pkg/ruby-rubocop-packaging) (0.3.0-1) - Shouldn't check `lib/` and `gemspec` file.  
- [bidi-clojure](https://tracker.debian.org/pkg/bidi-clojure) (2.1.3-1) - New upstream version for [`Puppet6`](https://wiki.debian.org/Teams/Puppet/Work).
- Source-only uploads for [ruby-anima](https://tracker.debian.org/pkg/ruby-anima), [ruby-uniform-notifier](https://tracker.debian.org/pkg/ruby-uniform-notifier), [ruby-unparser](https://tracker.debian.org/pkg/ruby-unparser), [ruby-morpher](https://tracker.debian.org/pkg/ruby-morpher), and [ruby-path-expander](https://tracker.debian.org/pkg/ruby-path-expander).

#### Other $things:

- Mentoring for newcomers.
- FTP Trainee reviewing.
- Moderation of -project mailing list.
- Sponsored `php-dasprid-enum` and `php-bacon-baconqrcode` for William and `ruby-unparser`, `ruby-morpher`, and `ruby-path-exapander` for Cocoa.

---

## Goodbye GSoC! \o/
![](/images/debian_ruby.png#center)

In May, I got selected as a [Google Summer of Code](https://summerofcode.withgoogle.com/) student for [Debian](https://www.debian.org/) again! \o/  
I am working on the [Upstream-Downstream Cooperation in Ruby](https://wiki.debian.org/SummerOfCode2020/Projects/#SummerOfCode2020.2FApprovedProjects.2FUpstreamDownstreamCooperationInRuby.Upstream.2FDownstream_cooperation_in_Ruby) project.

The other 5 blogs can be found here:
- [GSoC Phase 1 (part 1)](https://utkarsh2102.com/posts/gsoc-phase-1/).
- [GSoC Phase 1 (part 2)](https://utkarsh2102.com/posts/foss-in-june-20/).
- [GSoC Phase 2 (part 1)](https://utkarsh2102.com/posts/gsoc-phase-2/).
- [GSoC Phase 2 (part 2)](https://utkarsh2102.com/posts/foss-in-july-20/).
- [GSoC Phase 3 (part 1)](https://utkarsh2102.com/posts/gsoc-phase-3/).
- And this is GSoC Phase 3 (part 2).

Also, I log daily updates at [gsocwithutkarsh2102.tk](https://gsocwithutkarsh2102.tk/).

Since this is a wrap and whilst the daily updates are already available at the above site^, I'll quickly mention the important points and links here.

- The git repository is hosted on GitHub: https://github.com/utkarsh2102/rubocop-packaging.
- It is a linter, an extension of RuboCop, focused on enforcing upstream best practices and coding conventions.
- There have been 5 releases in all, including 4 cops and other bug fixes (including false-positives and false-negatives).
- The entire source code is documented with a separate `docs/` directory, which is hosted at https://docs.rubocop.org/rubocop-packaging.
- The packaging style guide is hosted at https://packaging.rubystyle.guide.
- At the time of writing this, it is being used by around 30 other projects ^.^
- Not only could you install this via [`gem install rubocop-packaging`](https://rubygems.org/gems/rubocop-packaging), but also via [`apt install ruby-rubocop-packaging`](https://tracker.debian.org/pkg/ruby-rubocop-packaging).
- The total work consists of [around 85 commits](https://github.com/utkarsh2102/rubocop-packaging/commits/master) with [15 PRs](https://github.com/utkarsh2102/rubocop-packaging/pulls?q=is%3Apr+is%3Aclosed), contributed by [4 amazing people](https://github.com/utkarsh2102/rubocop-packaging/graphs/contributors) (including me :P) in the last 3 months (June '20 to August '20).
- And finally, many thanks to two amazing people (the mentors for this project), [Antonio Terceiro](https://github.com/terceiro) and [David Rodríguez](https://github.com/deivid-rodriguez/)! 💖

![](/images/gsoc_meetings.png#center)

---

## Continuation of GSoC for other Ruby related stuff!
{{< figure src="/images/ruby-logo-small.png" >}}

Whilst working on [Rubocop::Packaging](https://github.com/utkarsh2102/rubocop-packaging), I contributed to more Ruby projects, refactoring their library a little bit and mostly fixing RuboCop issues and fixing issues that the `Packaging` extension reports as "offensive".  
Following are the PRs that I raised:

- [PR #170](https://github.com/ai/autoprefixer-rails/pull/170) for [autoprefixer-rails](https://github.com/ai/autoprefixer-rails) to drop `git ls-files` in gemspec.
- [PR #479](https://github.com/cucumber/cucumber-rails/pull/479) for [cucumber-rails](https://github.com/cucumber/cucumber-rails) to update `RuboCop` and `RuboCop::Packaging`.
- [PR #1465](https://github.com/cucumber/cucumber-ruby/pull/1465) for [cucumber-ruby](https://github.com/cucumber/cucumber-ruby) for updating `RuboCop` to v0.89.
- [PR #208](https://github.com/cucumber/cucumber-ruby-core/pull/208) for [cucumber-ruby-core](https://github.com/cucumber/cucumber-ruby-core) to fix `.rubocop.yml` and add `RuboCop::Packaging` as a development dependency.
- [PR #178](https://github.com/titusfortner/webdrivers/pull/178) for [webdrivers](https://github.com/titusfortner/webdrivers) to update the `RuboCop` and `RuboCop::RSpec` version to the latest.
- [PR #179](https://github.com/titusfortner/webdrivers/pull/179) for [webdrivers](https://github.com/titusfortner/webdrivers) to drop `git ls-files` in gemspec.

---

## Debian (E)LTS
{{< figure src="/images/debian-lts-small.png" >}}

[Debian Long Term Support (LTS)](https://www.freexian.com/en/services/debian-lts.html) is a project to extend the lifetime of all Debian stable releases to (at least) 5 years. Debian LTS is not handled by the Debian security team, but by a separate group of volunteers and companies interested in making it a success.  

And [Debian Extended LTS (ELTS)](https://deb.freexian.com/extended-lts) is its sister project, extending support to the Jessie release (+2 years after LTS support).

This was my eleventh month as a Debian LTS and my second as a Debian ELTS paid contributor.  
I was assigned 21.75 hours for LTS and 14.25 hours for ELTS and worked on
the following things:

#### LTS CVE Fixes and Announcements:

- Issued [DLA 2304-1](https://lists.debian.org/debian-lts-announce/2020/08/msg00000.html), fixing [CVE-2015-9542](https://security-tracker.debian.org/tracker/CVE-2015-9542), for [libpam-radius-auth](https://tracker.debian.org/pkg/libpam-radius-auth).  
  For Debian 9 Stretch, these problems have been fixed in version 1.3.16-5+deb9u1.
- Issued [DLA 2305-1](https://lists.debian.org/debian-lts-announce/2020/08/msg00001.html), fixing [CVE-2018-10756](https://security-tracker.debian.org/tracker/CVE-2018-10756), for [transmission](https://tracker.debian.org/pkg/transmission).  
  For Debian 9 Stretch, these problems have been fixed in version 2.92-2+deb9u2.
- Issued [DLA 2307-1](https://lists.debian.org/debian-lts-announce/2020/08/msg00002.html), fixing [CVE-2018-1000544](https://security-tracker.debian.org/tracker/CVE-2018-1000544), for [ruby-zip](https://tracker.debian.org/pkg/ruby-zip).  
  For Debian 9 Stretch, these problems have been fixed in version 1.2.0-1.1+deb9u1.
- Issued [DLA 2308-1](https://lists.debian.org/debian-lts-announce/2020/08/msg00003.html), fixing [CVE-2019-17113](https://security-tracker.debian.org/tracker/CVE-2019-17113), for [libopenmpt](https://tracker.debian.org/pkg/libopenmpt).  
  For Debian 9 Stretch, these problems have been fixed in version 0.2.7386~beta20.3-3+deb9u4.
- Issued [DLA 2317-1](https://lists.debian.org/debian-lts-announce/2020/08/msg00012.html), fixing [CVE-2020-10177](https://security-tracker.debian.org/tracker/CVE-2020-10177), for [pillow](https://tracker.debian.org/pkg/pillow).  
  For Debian 9 Stretch, these problems have been fixed in version 4.0.0-4+deb9u2.
- Issued [DLA 2318-1](https://lists.debian.org/debian-lts-announce/2020/08/msg00013.html), fixing [CVE-2019-10064](https://security-tracker.debian.org/tracker/CVE-2019-10064) and [CVE-2020-12695](https://security-tracker.debian.org/tracker/CVE-2020-12695), for [wpa](https://tracker.debian.org/pkg/wpa).  
  For Debian 9 Stretch, these problems have been fixed in version 2:2.4-1+deb9u7.
- Started working on [uwsgi](https://tracker.debian.org/pkg/uwsgi) update for [CVE-2020-11984](https://security-tracker.debian.org/tracker/CVE-2020-11984). It seems that src:apache2 wasn't affected by that, but src:uwsgi was.

#### ELTS CVE Fixes and Announcements:

- Issued [ELA 255-1](https://deb.freexian.com/extended-lts/updates/ela-255-1-libx11), fixing [CVE-2020-14344](https://security-tracker.debian.org/tracker/CVE-2020-14344), for [libx11](https://tracker.debian.org/pkg/libx11).  
  For Debian 8 Jessie, these problems have been fixed in version 2:1.6.2-3+deb8u3.
- Issued [ELA 259-1](https://deb.freexian.com/extended-lts/updates/ela-259-1-pillow), fixing [CVE-2020-10177](https://security-tracker.debian.org/tracker/CVE-2020-10177), for [pillow](https://tracker.debian.org/pkg/pillow).  
  For Debian 8 Jessie, these problems have been fixed in version 2.6.1-2+deb8u5.
- Issued [ELA 269-1](https://deb.freexian.com/extended-lts/updates/ela-269-1-apache2), fixing [CVE-2020-11985](https://security-tracker.debian.org/tracker/CVE-2020-11985), for [apache2](https://tracker.debian.org/pkg/apache2).  
  For Debian 8 Jessie, these problems have been fixed in version 2.4.10-10+deb8u17.
- Started working on [clamAV](https://tracker.debian.org/pkg/clamav) update, it's a major bump from v0.101.5 to v0.102.4. There were lots of movings parts. Contacted upstream maintainers to help reduce the risk of regression. Came up with a patch to loosen the libcurl version requirement. Hopefully, the update could be rolled out soon!

#### Other (E)LTS Work:

- I spent an additional 11.15 hours working on compiling the responses of the LTS survey and preparing a gist of it for its presentation during the Debian LTS BoF at DebConf20.
- Triaged [qemu](https://tracker.debian.org/pkg/qemu),
[pillow](https://tracker.debian.org/pkg/pillow),
[gupnp](https://tracker.debian.org/pkg/gupnp),
[clamav](https://tracker.debian.org/pkg/clamav),
[apache2](https://tracker.debian.org/pkg/apache2), and
[uwsgi](https://tracker.debian.org/pkg/uwsgi).
- Marked CVE-2020-11538/pillow as not-affected for Stretch.
- Marked CVE-2020-11984/apache2 as not-affected for Stretch.
- Marked CVE-2020-10378/pillow as not-affected for Jessie.
- Marked CVE-2020-11538/pillow as not-affected for Jessie.
- Marked CVE-2020-3481/clamav as not-affected for Jessie.
- Marked CVE-2020-11984/apache2 as not-affected for Jessie.
- Marked CVE-2020-{9490,11993}/apache2 as not-affected for Jessie.
- Hosted Debian LTS BoF at DebConf20. Recording [here](https://caesar.ftp.acc.umu.se/pub/debian-meetings/2020/DebConf20/72-debian-lts-bof.webm).
- General discussion on LTS private and [public mailing list](https://lists.debian.org/debian-lts/2020/08/threads.html).

---

Until next time.  
`:wq` for today.
