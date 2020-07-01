+++
date = "2020-07-01 09:30:00 +0530"
title = "FOSS Activites in June 2020"
slug = "foss-in-june-20"
images = [
    "/images/debian-logo-small.png",
    "/images/debian_ruby.png",
    "/images/bbatsov-comment.png",
    "/images/lienvdsteen-comment.png",
    "/images/pboling-comment.png",
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

Here's my (ninth) monthly update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 16th month of contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March last year and a [DD](https://wiki.debian.org/DebianDeveloper) last Christmas! \o/  

This month was a little intense. I did a a lot of different kinds of things in Debian this month. Whilst most of my time went on doing security stuff, I also sponosred a bunch of packages.

Here are the following things I did this month:

#### Uploads and bug fixes:

- [rails](https://tracker.debian.org/pkg/rails) (2:5.2.4.3+dfsg-1) - fix a bunch of [CVEs](https://security-tracker.debian.org/tracker/source-package/rails) in Sid and Bullseye.  
- [ruby-json](https://tracker.debian.org/pkg/ruby-json) (2.1.0+dfsg-2+deb10u1) - backport [CVE-2020-10663](https://security-tracker.debian.org/tracker/CVE-2020-10663) fix to Buster.  
- [ruby-json](https://tracker.debian.org/pkg/ruby-json) (2.0.1+dfsg-3+deb9u1) - backport [CVE-2020-10663](https://security-tracker.debian.org/tracker/CVE-2020-10663) fix to Stretch.  
- [ruby-kaminari](https://tracker.debian.org/pkg/ruby-kaminari) (1.0.1-6) - add patch to fix [CVE-2020-11082](https://security-tracker.debian.org/tracker/CVE-2020-11082).  
- [ruby2.3](https://tracker.debian.org/pkg/ruby2.3) (2.3.3-1+deb9u8) - backport [CVE-2020-10663](https://security-tracker.debian.org/tracker/CVE-2020-10663) fix to Stretch.  
- [python-libusb1](https://tracker.debian.org/pkg/python-libusb1) (1.8-1.1) - NMU for a source-only upload.  
- [pry](https://tracker.debian.org/pkg/pry) (0.13.1-1) - Fix failing tests & new upstream version.  
- [ruby-rubocop-packaging](https://tracker.debian.org/pkg/ruby-rubocop-packaging) (0.1.0-1) - NEW ([#963016](bugs.debian.org/963016)).  
- [batalert](https://tracker.debian.org/pkg/batalert) (0.4.0-1) - fixes against RuboCop.  
- [json-schema-test-suite](https://tracker.debian.org/pkg/json-schema-test-suite) (2.0.0-1.1) - NMU for a source-only upload on request.  
- [ruby-ahoy-email](https://tracker.debian.org/pkg/ruby-ahoy-email) (1.1.0-1) - Disable tests temporarily ([#959060](bugs.debian.org/959060)).  
- [micro](https://tracker.debian.org/pkg/micro) (2.0.6-1) - fix crashing at startup ([#961853](bugs.debian.org/961853)).  
- [golang-github-zyedidia-tcell](https://tracker.debian.org/pkg/golang-github-zyedidia-tcell) (1.4.8-1) - new upstream version.  
- [micro](https://tracker.debian.org/pkg/micro) (2.0.6-1~bpo10+1) - backport the fix for ([#961853](bugs.debian.org/961853)).  
- [micro](https://tracker.debian.org/pkg/micro) (2.0.6-2) - fix the reintroduced versioning issue ([#953400](bugs.debian.org/953400)).  
- [ruby-whitequark-parser](https://tracker.debian.org/pkg/ruby-whitequark-parser) (2.7.1.4-1) - new upstream version.  

#### Other $things:

- Hosted Ruby team meeting. Logs [here](http://meetbot.debian.net/debian-ruby/2020/debian-ruby.2020-06-05-16.41.html).  
- Mentoring for newcomers.  
- FTP Trainee reviewing.  
- Moderation of -project mailing list.  
- Sponsored `ruby-ast` for Abraham, `libexif` for Hugh, `djangorestframework-gis` and `karlseguin-ccache` for Nilesh, and `twig-extensions`, `twig-i18n-extension`, and `mariadb-mysql-kbs` for William.  

---

## GSoC Phase 1, Part 2!
![](/images/debian_ruby.png#center)

Last month, I got selected as a [Google Summer of Code](https://summerofcode.withgoogle.com/) student for [Debian](https://www.debian.org/) again! \o/  
I am working on the [Upstream-Downstream Cooperation in Ruby](https://wiki.debian.org/SummerOfCode2020/Projects/#SummerOfCode2020.2FApprovedProjects.2FUpstreamDownstreamCooperationInRuby.Upstream.2FDownstream_cooperation_in_Ruby) project.

The first half of the first month is blogged here, titled, [GSoC Phase 1](https://utkarsh2102.com/posts/gsoc-phase-1/).  
Also, I log daily updates at [gsocwithutkarsh2102.tk](https://gsocwithutkarsh2102.tk/).

Whilst the daily updates are available at the above site^, I’ll breakdown the important parts of the later half of the first month here:

- Documented the first cop, `GemspecGit` via [PR #2](https://github.com/utkarsh2102/rubocop-packaging/pull/2).
- Made an initial release, [v0.1.0](https://rubygems.org/gems/rubocop-packaging)! 💖
- Spread the word/usage about this tool/library via adding them in the official [RuboCop docs](https://docs.rubocop.org/rubocop/extensions.html).
- We had our [third weekly meeting](https://gsocwithutkarsh2102.tk/log/2020/06/18/day18.html) where we discussed the next steps and the things that are supposed to be done for the next set of cops.
- Wrote more tests so as to cover different aspects of the `GemspecGit` cop.
- Opened [PR #4](https://github.com/utkarsh2102/rubocop-packaging/pull/4/) for the next Cop, `RequireRelativeToLib`.
- Introduced [rubocop-packaging](https://github.com/utkarsh2102/rubocop-packaging) to the outer world and requested other upstream projects to use it! It is being used by 6 other projects already 😭💖
- Had our [fourth weekly meeting](https://gsocwithutkarsh2102.tk/log/2020/06/25/day25.html) where we pair-programmed (and I sucked :P) and figured out a way to make the second cop work.
- Found a bug, reported at [issue #5](https://github.com/utkarsh2102/rubocop-packaging/issues/5) and raised [PR #6](https://github.com/utkarsh2102/rubocop-packaging/pull/6) to fix it.
- And finally, people loved the library/tool (and it's outcome):
![](/images/bbatsov-comment.png#center)  
![](/images/lienvdsteen-comment.png#center)  
![](/images/pboling-comment.png#center)  
(for those who don't know, [@bbatsov](https://github.com/bbatsov) is the author of [RuboCop](https://rubocop.org/), [@lienvdsteen](https://gitlab.com/lienvdsteen) is an amazing fullstack engineer at GitLab, and [@pboling](https://github.com/pboling) is the author of some awesome Ruby tools and libraries!)

---

Thank you for sticking along for so long :)  

Until next time.  
`:wq` for today.
