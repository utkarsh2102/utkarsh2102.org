+++
date = "2020-06-30 09:30:00 +0530"
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

This month was a little intense. I did a lot of different kinds of things in Debian this month. Whilst most of my time went on doing security stuff, I also sponsored a bunch of packages.

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

## Continuation of GSoC for other Ruby related stuff!
{{< figure src="/images/ruby-logo-small.png" >}}

Whilst I have already mentioned it multiple times but it's still not enough to stress how amazing [Antonio Terceiro](https://github.com/terceiro) and [David Rodríguez](https://github.com/deivid-rodriguez/) are! 💖  
They're more than just mentors to me!

Well, only they know how much I trouble them with different things, which are not only related to my GSoC project but also extends to the projects they maintain! :P  
David maintains [rubygems and bundler](https://github.com/rubygems/rubygems/) and Antonio maintains [debci](https://salsa.debian.org/ci-team/debci).

So on days when I decide to hack on `rubygems` or `debci`, only I know how kind and nice David and Anotonio are to me!  
They very patiently walk me through with whatever I am stuck on, no matter what and no matter when.

Thus, with them around, I contributed to these two projects and more, with regards to working on `rubocop-packaging`.  
Following are a few things that I raised:

- [PR #3731](https://github.com/rubygems/rubygems/pull/3731) for [rubygems/bundler](https://github.com/rubygems/rubygems) to ship default `.rubocop.yml` file.
- [PR #2140](https://github.com/pry/pry/pull/2140) for [pry](https://github.com/pry/pry) to fix `bundler_spec` test.
- [PR #3740](https://github.com/rubygems/rubygems/pull/3740) for [rubygems/bundler](https://github.com/rubygems/rubygems) to fix all RuboCop offenses.
- [MR #114](https://salsa.debian.org/ci-team/debci/-/merge_requests/114) for [debci](https://salsa.debian.org/ci-team/debci) to show package details on the retry page.
- [Issue #356](https://github.com/ruby/rake/issues/356) against [rake](https://github.com/ruby/rake) to request to support all `gitignore` rule patterns in `rake/file_list`.
- [PR #9](https://github.com/robotdana/fast_ignore/pull/9) for [fast_ignore](https://github.com/robotdana/fast_ignore) to use `fast_ignore` instead of `git ls-files`.
- [PR #3748](https://github.com/rubygems/rubygems/pull/3748) for [rubygems/bundler](https://github.com/rubygems/rubygems) to add actions to automatically bump man page month.
- [PR #8160](https://github.com/rubocop-hq/rubocop/pull/8160) for [rubocop](https://github.com/rubocop-hq/rubocop) to add `rubocop-packaging` as a known extension.
- [PR #3754](https://github.com/rubygems/rubygems/pull/3754) for [rubygems/bundler](https://github.com/rubygems/rubygems) to constrain the shipped RuboCop's version.
- [Issue #8](https://github.com/robotdana/fast_ignore/issues/8) against [fast_ignore](https://github.com/robotdana/fast_ignore) to clarify the strange behavior of `include_files`.
- [PR #3765](https://github.com/rubygems/rubygems/pull/3765) for [rubygems/bundler](https://github.com/rubygems/rubygems) to fix remaining RuboCop issues and add tests.


---

## Debian LTS
{{< figure src="/images/debian-lts-small.png" >}}

Debian Long Term Support (LTS) is a project to extend the lifetime of all Debian stable releases
to (at least) 5 years. Debian LTS is not handled by the Debian security team, but by a separate group
of volunteers and companies interested in making it a success.  

This was my ninth month as a Debian LTS paid contributor. I was assigned 30.00 hours and worked on
the following things:  

#### CVE Fixes and Announcements:

- Issued [DLA 2215-1](https://lists.debian.org/debian-lts-announce/2020/05/msg00018.html), fixing [CVE-2020-3327](https://security-tracker.debian.org/tracker/CVE-2020-3327) and [CVE-2020-3341](https://security-tracker.debian.org/tracker/CVE-2020-3341), for [clamav](https://tracker.debian.org/clamav).  
  For Debian 8 "Jessie", these problems have been fixed in version 0.101.5+dfsg-0+deb8u2.

- Issued [DLA 2216-1](https://lists.debian.org/debian-lts-announce/2020/05/msg00019.html), fixing [CVE-2020-8161](https://security-tracker.debian.org/tracker/CVE-2020-8161), for [ruby-rack](https://tracker.debian.org/ruby-rack).  
  For Debian 8 "Jessie", this problem has been fixed in version 1.5.2-3+deb8u3.

- Issued [DLA 2234-1](https://lists.debian.org/debian-lts-announce/2020/06/msg00002.html), fixing [CVE-2005-1513](https://security-tracker.debian.org/tracker/CVE-2005-1513), [CVE-2005-1514](https://security-tracker.debian.org/tracker/CVE-2005-1514), [CVE-2005-1515](https://security-tracker.debian.org/tracker/CVE-2005-1515), [CVE-2020-3811](https://security-tracker.debian.org/tracker/CVE-2020-3811), and [CVE-2020-3812](https://security-tracker.debian.org/tracker/CVE-2020-3812), for [netqmail](https://tracker.debian.org/netqmail).  
  For Debian 8 "Jessie", these problems have been fixed in version 1.06-6.2~deb8u1.

- Uploaded a fix for [CVE-2020-8162](https://security-tracker.debian.org/tracker/CVE-2020-8162), [CVE-2020-8164](https://security-tracker.debian.org/tracker/CVE-2020-8164), [CVE-2020-8165](https://security-tracker.debian.org/tracker/CVE-2020-8165), [CVE-2020-8166](https://security-tracker.debian.org/tracker/CVE-2020-8166), and [CVE-2020-8167](https://security-tracker.debian.org/tracker/CVE-2020-8167), for [rails](https://tracker.debian.org/rails).
  This upload was for Sid and Bullseye and these CVE(s) were fixed in version 2:5.2.4.3+dfsg-1.

- Uploaded a fix for [CVE-2020-11082](https://security-tracker.debian.org/tracker/CVE-2020-11082), for [ruby-kaminari](https://tracker.debian.org/ruby-kaminari).
  This upload was for Sid and Bullseye and this CVE was fixed in version 1.0.1-6.

- Uploaded a fix for [CVE-2020-10663](https://security-tracker.debian.org/tracker/CVE-2020-10663), for [ruby-json](https://tracker.debian.org/ruby-json), [ruby2.1](https://tracker.debian.org/ruby2.1), and [ruby2.5](https://tracker.debian.org/ruby2.5).
  These uploads were for Stretch and Buster and were fixed in the version 2.3.3-1+deb9u8, 2.1.0+dfsg-2+deb10u1, 2.3.3-1+deb9u8, and 2.5.5-3+deb10u2.

- Issued [DLA 2237-1](https://lists.debian.org/debian-lts-announce/2020/06/msg00005.html), fixing [CVE-2019-8842](https://security-tracker.debian.org/tracker/CVE-2019-8842) and [CVE-2020-3898](https://security-tracker.debian.org/tracker/CVE-2020-3898), for [cups](https://tracker.debian.org/cups).  
  For Debian 8 "Jessie", these problems have been fixed in version 1.7.5-11+deb8u8.

- Issued [DLA 2246-1](https://lists.debian.org/debian-lts-announce/2020/06/msg00018.html), fixing [CVE-2020-13696](https://security-tracker.debian.org/tracker/CVE-2020-13696), for [xawtv](https://tracker.debian.org/xawtv).  
  For Debian 8 "Jessie", this problem has been fixed in version 3.103-3+deb8u1.

- Issued [DLA 2248-1](https://lists.debian.org/debian-lts-announce/2020/06/msg00019.html), fixing [CVE-2020-0543](https://security-tracker.debian.org/tracker/CVE-2020-0543), [CVE-2020-0548](https://security-tracker.debian.org/tracker/CVE-2020-0548), and [CVE-2020-0549](https://security-tracker.debian.org/tracker/CVE-2020-0549), for [intel-microcode](https://tracker.debian.org/intel-microcode).  
  For Debian 8 "Jessie", these problems have been fixed in version 3.20200609.2~deb8u1.

- Issued [DLA 2249-1](https://lists.debian.org/debian-lts-announce/2020/06/msg00020.html), fixing [CVE-2020-0182](https://security-tracker.debian.org/tracker/CVE-2020-0182) and [CVE-2020-0198](https://security-tracker.debian.org/tracker/CVE-2020-0198), for [libexif](https://tracker.debian.org/libexif).  
  For Debian 8 "Jessie", these problems have been fixed in version 0.6.21-2+deb8u4.

#### Other LTS Work:

- Triaged [sympa](https://tracker.debian.org/pkg/sympa),
[apache2](https://tracker.debian.org/pkg/apache2),
[qemu](https://tracker.debian.org/pkg/qemu), and
[coturn](https://tracker.debian.org/pkg/coturn).
- Add fix for CVE-2020-0198/libexif.
- Requested CVE for [bug#60251](https://bz.apache.org/bugzilla/show_bug.cgi?id=60251) against [apache2](https://tracker.debian.org/pkg/apache2) and prodded further.
- Raised [issue #947](https://github.com/sympa-community/sympa/issues/947) against `sympa` reporting an incomplete patch for CVE-2020-10936. More discussions internally.
- Created the LTS Survey on the self-hosted LimeSurvey instance.
- Attended the third LTS meeting. Logs [here](http://meetbot.debian.net/debian-lts/2020/debian-lts.2020-06-25-15.22.html).
- General discussion on LTS private and [public mailing list](https://lists.debian.org/debian-lts/2020/05/threads.html).

---

## Other(s)
{{< figure src="/images/computing.jpg" >}}

Sometimes it gets hard to categorize work/things into a particular category.  
That's why I am writing all of those things inside this category.  
This includes two sub-categories and they are as follows.

#### Personal:

This month I did the following things:

- Wrote and published v0.1.0 of `rubocop-packaging` on [RubyGems](https://rubygems.org/gems/rubocop-packaging)! 💯  
  It's open-sourced and the repository is [here](https://github.com/utkarsh2102/rubocop-packaging).  
  Bug reports and pull requests are welcomed! 😉
- Integrated a tiny (yet a powerful) hack to align images in markdown for my blog.  
  Commit [here](https://github.com/utkarsh2102/hugo-coder/commit/646aed40da8d508dbeaa8d8698b65212574a136a). 🚀
- Released v0.4.0 of `batalert` on [RubyGems](https://rubygems.org/gems/batalert)! 🤗  

#### Open Source:

Again, this contains all the things that I couldn't categorize earlier.  
Opened several issues and PRs:

- [Issue #9](https://github.com/FabioRosado/100daysof/issues/9) against [100daysof](https://github.com/FabioRosado/100daysof), reporting some broken CSS.
- [PR #10](https://github.com/FabioRosado/100daysof/pull/10) for [100daysof](https://github.com/FabioRosado/100daysof), fixing the above issue^.
- [Issue #133](https://github.com/florimondmanca/djangorestframework-api-key/issues/133) against [djangorestframework-api-key](https://github.com/florimondmanca/djangorestframework-api-key), asking to fix copyright years.
- [PR #5](https://github.com/pboling/rspec-stubbed_env/pull/5) for [rspec-stubbed_env](https://github.com/pboling/rspec-stubbed_env), dropping `git ls-files` in gemspec.
- [PR #70](https://github.com/pboling/rspec-pending_for/pull/70) for [rspec-pending_for](https://github.com/pboling/rspec-pending_for), dropping `git ls-files` in gemspec.
- [Issue #74](https://github.com/podigee/device_detector/issues/74), [issue #143](https://github.com/ankane/ahoy_email/issues/143), [issue #164](https://github.com/ai/autoprefixer-rails/issues/164), and [issue #767](https://github.com/ddollar/foreman/issues/767) against multiple projects, asking them to use RuboCop.
- [PR #212](https://github.com/activeadmin/arbre/pull/212) for [arbre](https://github.com/activeadmin/arbre), dropping `git ls-files` in gemspec.
- [Issue #1749](https://github.com/zyedidia/micro/issues/1749) and [issue #1750](https://github.com/zyedidia/micro/issues/1750) against [micro](https://github.com/zyedidia/micro), asking for help as the Debian package fails to build in `buster-backports`.
- [PR #1751](https://github.com/zyedidia/micro/pull/1751) for [micro](https://github.com/zyedidia/micro/pull/1751), fixing the above issue^.
- [Issue #348](https://github.com/luizdepra/hugo-coder/issues/348) against [hugo-coder](https://github.com/luizdepra/hugo-coder), clarifying the weird timing issue in the blog posts.
- [Issue #356](https://github.com/luizdepra/hugo-coder/issues/356) against [hugo-coder](https://github.com/luizdepra/hugo-coder), reporting the weird display of images and missing twitter cards.
- [MR #12](https://gitlab.com/lienvdsteen/linter/-/merge_requests/12) for [linter](https://gitlab.com/lienvdsteen/linter), dropping `git ls-files` in gemspec.
- [MR #13](https://gitlab.com/lienvdsteen/linter/-/merge_requests/13) for [linter](https://gitlab.com/lienvdsteen/linter), doing so minor refactoring.

---

Thank you for sticking along for so long :)  

Until next time.  
`:wq` for today.
