+++
date = "2020-08-01 14:30:00 +0530"
title = "FOSS Activites in July 2020"
slug = "foss-in-july-20"
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

Here's my (tenth) monthly update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 17th month of contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March last year and a [DD](https://wiki.debian.org/DebianDeveloper) last Christmas! \o/  

Well, this month I didn't do a lot of Debian stuff, like I usually do, however, I did a lot of things related to Debian (indirectly via GSoC)!

Anyway, here are the following things I did this month:

#### Uploads and bug fixes:

- [rails](https://tracker.debian.org/pkg/rails) (2:6.0.3.2+dfsg-1) - Fix [CVE-2020-8185](https://security-tracker.debian.org/tracker/CVE-2020-8185) (Closes [#964081](https://bugs.debian.org/964081)).  
- [ruby-rubocop-packaging](https://tracker.debian.org/pkg/ruby-rubocop-packaging) (0.1.1-1) - Fix blank file [issue](https://github.com/utkarsh2102/rubocop-packaging/issues/5).  
- [micro](https://tracker.debian.org/pkg/micro) (2.0.6-2~bpo10+1) - Backport new upstream version.  
- [ruby2.5](https://tracker.debian.org/pkg/ruby2.5) (2.5.5-3+deb10u2) - Fix [CVE-2020-10663](https://security-tracker.debian.org/tracker/CVE-2020-10663) and [CVE-2020-10933](https://security-tracker.debian.org/tracker/CVE-2020-10933).  
- [djangorestframework-api-key](https://tracker.debian.org/pkg/djangorestframework-api-key) (2.0.0-2) - Fix [#956920](https://bugs.debian.org/956920).  
- [golang-golang-x-text](https://tracker.debian.org/pkg/golang-golang-x-text) (0.3.3-1~bpo10+1) - Backport [CVE-2020-14040](https://security-tracker.debian.org/tracker/CVE-2020-14040) fix to Buster.  
- [ruby-growl](https://tracker.debian.org/pkg/ruby-growl) (4.1+dfsg-2) - Source-only upload.  
- [ruby-iso8601](https://tracker.debian.org/pkg/ruby-iso8601) (0.13.0-1) - New upstream version, drop patches as they're merged upstream.  
- [sup-mail](https://tracker.debian.org/pkg/sup-mail) (1.0-1) - Re-introduce sup-mail to the Debian archive.  
- [ruby-rubocop-packaging](https://tracker.debian.org/pkg/ruby-rubocop-packaging) (0.2.0-1) - New version for the `RelativeRequireToLib` cop.  
- [ruby-rubocop-ast](https://tracker.debian.org/pkg/ruby-rubocop-ast) (0.1.0-2) - Source-only upload.  
- [ruby-rubocop-rspec](https://tracker.debian.org/pkg/ruby-rubocop-rspec) (1.42.0-1) - Fixing FTBFS with RuboCop v0.88.0 via v1.42.0.  
- [ruby-rubocop-performance](https://tracker.debian.org/pkg/ruby-rubocop-performance) (1.7.1-1) - Fixing FTBFS with RuboCop v0.88.0 via v1.7.1.  

#### Other $things:

- Mentoring for newcomers.  
- FTP Trainee reviewing.  
- Moderation of -project mailing list.  
- Sponsored `php-twig` for William, `ruby-growl`, `ruby-xmpp4r`, and `uby-uniform-notifier` for Cocoa, `sup-mail` for Iain, and `node-markdown-it` for Sakshi.

---

## GSoC Phase 2, Part 2!
![](/images/debian_ruby.png#center)

In May, I got selected as a [Google Summer of Code](https://summerofcode.withgoogle.com/) student for [Debian](https://www.debian.org/) again! \o/  
I am working on the [Upstream-Downstream Cooperation in Ruby](https://wiki.debian.org/SummerOfCode2020/Projects/#SummerOfCode2020.2FApprovedProjects.2FUpstreamDownstreamCooperationInRuby.Upstream.2FDownstream_cooperation_in_Ruby) project.

The first three blogs can be found here:
- [GSoC Phase 1 (part 1)](https://utkarsh2102.com/posts/gsoc-phase-1/).
- [GSoC Phase 1 (part 2)](https://utkarsh2102.com/posts/foss-in-june-20/).
- [GSoC Phase 2 (part 1)](https://utkarsh2102.com/posts/gsoc-phase-2/).
- And this is GSoC Phase 2 (part 2).

Also, I log daily updates at [gsocwithutkarsh2102.tk](https://gsocwithutkarsh2102.tk/).

Whilst the daily updates are available at the above site^, I’ll breakdown the important parts of the later half of the second month here:

- [Marc Andre](https://github.com/marcandre), very kindly, helped in [fixing the specs](https://github.com/marcandre/rubocop-packaging/commit/90d23d16dff4fd00652d3e5c7f32c88d9c987225) that were failing earlier this month. Well, the problem was with the specs, but I am still confused how so. Anyway..
- Finished documentation of the second cop and marked the PR as ready to be reviewed.
- David reviewed and suggested some really good changes and I fixed/tweaked that PR as per his suggestion to finally finish the last bits of the second cop, `RelativeRequireToLib`.
- Merged the PR upon two approvals and released it as v0.2.0! 💖
- We had our next weekly meeting where we discussed the next steps and the things that are supposed to be done for the next set of cops.
- Introduced [rubocop-packaging](https://github.com/utkarsh2102/rubocop-packaging) to the outer world and requested other upstream projects to use it! It is being used by [13 other projects](https://github.com/utkarsh2102/rubocop-packaging/network/dependents?package_id=UGFja2FnZS0xMjY1ODQyMzQ1) already! 😭💖
- Started to work on [packaging-style-guide](https://github.com/utkarsh2102/packaging-style-guide) but I didn't push anything to the public repository yet.
- Worked on refactoring the `cops_documentation` Rake task which was broken by the new auto-corrector API. Opened [PR #7](https://github.com/utkarsh2102/rubocop-packaging/pull/7) for it. It'll be merged after the next RuboCop release as it uses `CopsDocumentationGenerator` class from the master branch.
- Whilst working on [autoprefixer-rails](https://github.com/ai/autoprefixer-rails), I found something unusual. The second cop shouldn't really report offenses if the `require_relative` calls are from `lib` to `lib` itself. This is a false-positive. Opened [issue #8](https://github.com/utkarsh2102/rubocop-packaging/issues/8) for the same.

---

## Continuation of GSoC for other Ruby related stuff!
{{< figure src="/images/ruby-logo-small.png" >}}

Whilst working on `rubocop-packaging`, I contributed to more Ruby projects, refactoring their library a little bit and mostly fixing RuboCop issues and fixing issues that the `Packaging` extension reports as "offensive".  
Following are the PRs that I raised:

- [PR #175](https://github.com/mvz/gir_ffi/pull/175) for [gir_ffi](https://github.com/mvz/gir_ffi) to drop `git ls-files` in gemspec.
- [PR #3791](https://github.com/rubygems/rubygems/pull/3791) for [rubygems/bundler](https://github.com/rubygems/rubygems) to remove redundant `bundler/setup` require call from `spec_helper` generated by `bundle gem`.
- [PR #2307](https://github.com/puma/puma/pull/2307) for [puma](https://github.com/puma/puma) to constrain `rake-compiler` to v0.9.4.
- [PR #476](https://github.com/cucumber/cucumber-rails/pull/476) for [cucumber-rails](https://github.com/cucumber/cucumber-rails) to drop `git ls-files` in gemspec.
- [PR #721](https://github.com/cucumber/aruba/pull/721) for [aruba](https://github.com/cucumber/aruba) to drop `git ls-files` in gemspec.
- [PR #89](https://github.com/savonrb/wasabi/pull/89) for [wasabi](https://github.com/savonrb/wasabi) to drop `git ls-files` in gemspec.
- [PR #24](https://github.com/RubyCrypto/ed25519/pull/24) for [ed25519](https://github.com/RubyCrypto/ed25519) to fix RuboCop warning and offenses.
- [PR #25](https://github.com/RubyCrypto/ed25519/pull/25) for [ed25519](https://github.com/RubyCrypto/ed25519) to drop `git ls-files` in gemspec.
- [PR #59](https://github.com/arnau/ISO8601/pull/59) for [ISO8601](https://github.com/arnau/ISO8601) to drop `git ls-files` in gemspec.
- [PR #60](https://github.com/arnau/ISO8601/pull/60) for [ISO8601](https://github.com/arnau/ISO8601) to fix other RuboCop offenses.
- [PR #61](https://github.com/arnau/ISO8601/pull/61) for [ISO8601](https://github.com/arnau/ISO8601) to (minor) refactor the library.
- [PR #580](https://github.com/sup-heliotrope/sup/pull/580) for [sup](https://github.com/sup-heliotrope/sup) to drop `git ls-files` in gemspec.
- [PR #166](https://github.com/ai/autoprefixer-rails/pull/166) for [autoprefixer-rails](https://github.com/ai/autoprefixer-rails) to use RuboCop to enhance some bits of code.
- [PR #167](https://github.com/ai/autoprefixer-rails/pull/167) for [autoprefixer-rails](https://github.com/ai/autoprefixer-rails) to fix remaining RuboCop warning and offenses.
- [PR #169](https://github.com/ai/autoprefixer-rails/pull/169) for [autoprefixer-rails](https://github.com/ai/autoprefixer-rails) to do some minor refactoring.
- [PR #170](https://github.com/ai/autoprefixer-rails/pull/170) for [autoprefixer-rails](https://github.com/ai/autoprefixer-rails) to drop `git ls-files` in gemspec.

---

## Debian (E)LTS
{{< figure src="/images/debian-lts-small.png" >}}

Debian Long Term Support (LTS) is a project to extend the lifetime of all Debian stable releases to (at least) 5 years. Debian LTS is not handled by the Debian security team, but by a separate group of volunteers and companies interested in making it a success.  

And Debian Extended LTS (ELTS) is its sister project, extending support to the Jessie release (+2 years after LTS support).

This was my tenth month as a Debian LTS and my first as a Debian ELTS paid contributor.  
I was assigned 25.25 hours for LTS and 13.25 hours for ELTS and worked on
the following things:  

#### LTS CVE Fixes and Announcements:

- Issued [DLA 2269-1](https://lists.debian.org/debian-lts-announce/2020/07/msg00000.html), fixing [CVE-2020-4046](https://security-tracker.debian.org/tracker/CVE-2020-4046), [CVE-2020-4047](https://security-tracker.debian.org/tracker/CVE-2020-4047), [CVE-2020-4048](https://security-tracker.debian.org/tracker/CVE-2020-4048), [CVE-2020-4049](https://security-tracker.debian.org/tracker/CVE-2020-4049), and [CVE-2020-4050](https://security-tracker.debian.org/tracker/CVE-2020-4050), for [wordpress](https://tracker.debian.org/pkg/wordpress).  
  For Debian 8 Jessie, these problems have been fixed in version 4.1.31+dfsg-0+deb8u1.
- Issued [DLA 2270-1](https://lists.debian.org/debian-lts-announce/2020/07/msg00001.html), fixing [CVE-2020-14060](https://security-tracker.debian.org/tracker/CVE-2020-14060), [CVE-2020-14061](https://security-tracker.debian.org/tracker/CVE-2020-14061), [CVE-2020-14062](https://security-tracker.debian.org/tracker/CVE-2020-14062), and [CVE-2020-14195](https://security-tracker.debian.org/tracker/CVE-2020-14195), for [jackson-databind](https://tracker.debian.org/pkg/jackson-databind).  
  For Debian 8 Jessie, these problems have been fixed in version 2.4.2-2+deb8u15.
- Issued [DLA 2271-1](https://lists.debian.org/debian-lts-announce/2020/07/msg00002.html), fixing [CVE-2020-4067](https://security-tracker.debian.org/tracker/CVE-2020-4067), for [coturn](https://tracker.debian.org/pkg/coturn).  
  For Debian 8 Jessie, this problem has been fixed in version 4.2.1.2-1+deb8u2.
- Issued [DLA 2275-1](https://lists.debian.org/debian-lts-announce/2020/07/msg00006.html), fixing [CVE-2020-8161](https://security-tracker.debian.org/tracker/CVE-2020-8161) and [CVE-2020-8184](https://security-tracker.debian.org/tracker/CVE-2020-8184), for [ruby-rack](https://tracker.debian.org/pkg/ruby-rack).  
  For Debian 9 Stretch, these problems have been fixed in version 1.6.4-4+deb9u2.
- Issued [DLA 2276-1](https://lists.debian.org/debian-lts-announce/2020/07/msg00007.html), fixing [CVE-2020-12108](https://security-tracker.debian.org/tracker/CVE-2020-12108) and [CVE-2020-15011](https://security-tracker.debian.org/tracker/CVE-2020-15011), for [mailman](https://tracker.debian.org/pkg/mailman).  
  For Debian 9 Stretch, these problems have been fixed in version 1:2.1.23-1+deb9u6.
- Issued [DLA 2277-1](https://lists.debian.org/debian-lts-announce/2020/07/msg00008.html), fixing [CVE-2019-12973](https://security-tracker.debian.org/tracker/CVE-2019-12973), [CVE-2020-6851](https://security-tracker.debian.org/tracker/CVE-2020-6851), [CVE-2020-8112](https://security-tracker.debian.org/tracker/CVE-2020-8112), and [CVE-2020-15389](https://security-tracker.debian.org/tracker/CVE-2020-15389), for [openjpeg2](https://tracker.debian.org/pkg/openjpeg2).  
  For Debian 9 Stretch, these problems have been fixed in version 2.1.2-1.1+deb9u5.
- Issued [DLA 2288-1](https://lists.debian.org/debian-lts-announce/2020/07/msg00020.html), fixing [CVE-2017-9503](https://security-tracker.debian.org/tracker/CVE-2017-9503), [CVE-2019-12068](https://security-tracker.debian.org/tracker/CVE-2019-12068), [CVE-2019-20382](https://security-tracker.debian.org/tracker/CVE-2019-20382), [CVE-2020-1983](https://security-tracker.debian.org/tracker/CVE-2020-1983), [CVE-2020-8608](https://security-tracker.debian.org/tracker/CVE-2020-8608), [CVE-2020-10756](https://security-tracker.debian.org/tracker/CVE-2020-10756), [CVE-2020-13361](https://security-tracker.debian.org/tracker/CVE-2020-13361), [CVE-2020-13362](https://security-tracker.debian.org/tracker/CVE-2020-13362), [CVE-2020-13659](https://security-tracker.debian.org/tracker/CVE-2020-13659), [CVE-2020-13754](https://security-tracker.debian.org/tracker/CVE-2020-13754), [CVE-2020-13765](https://security-tracker.debian.org/tracker/CVE-2020-13765), and [CVE-2020-15863](https://security-tracker.debian.org/tracker/CVE-2020-15863), for [qemu](https://tracker.debian.org/pkg/qemu). This was mostly worked upon by the maintainer, Michael.  
  For Debian 9 Stretch, these problems have been fixed in version 1:2.8+dfsg-6+deb9u10.

#### ELTS CVE Fixes and Announcements:

- Issued [ELA 240-1](https://deb.freexian.com/extended-lts/updates/ela-240-1-wpa), fixing [CVE-2020-12695](https://security-tracker.debian.org/tracker/CVE-2020-12695), for [wpa](https://tracker.debian.org/pkg/wpa).  
  For Debian 8 Jessie, these problems have been fixed in version 2.3-1+deb8u11.
- Issued [ELA 241-1](https://deb.freexian.com/extended-lts/updates/ela-241-1-openjpeg2), fixing [CVE-2020-15389](https://security-tracker.debian.org/tracker/CVE-2020-15389), for [openjpeg2](https://tracker.debian.org/pkg/openjpeg2).  
  For Debian 8 Jessie, these problems have been fixed in version 2.1.0-2+deb8u11.
- Issued [ELA 249-1](https://deb.freexian.com/extended-lts/updates/ela-249-1-qemu), fixing [CVE-2020-13659](https://security-tracker.debian.org/tracker/CVE-2020-13659) and [CVE-2020-15863](https://security-tracker.debian.org/tracker/CVE-2020-15863), for [qemu](https://tracker.debian.org/pkg/qemu).  
  For Debian 8 Jessie, these problems have been fixed in version 1:2.1+dfsg-12+deb8u16.

#### Other (E)LTS Work:

- Did my LTS frontdesk duty from 29th June to 5th July.
- Triaged [qemu](https://tracker.debian.org/pkg/qemu),
[firefox-esr](https://tracker.debian.org/pkg/firefox-esr),
[wordpress](https://tracker.debian.org/pkg/wordpress),
[libmediainfo](https://tracker.debian.org/pkg/libmediainfo),
[squirrelmail](https://tracker.debian.org/pkg/squirrelmail),
[xen](https://tracker.debian.org/pkg/xen),
[openjpeg2](https://tracker.debian.org/pkg/openjpeg2),
[samba](https://tracker.debian.org/pkg/samba), and
[ldb](https://tracker.debian.org/pkg/ldb).
- Mark CVE-2020-15395/libmediainfo as no-dsa for Jessie.
- Mark CVE-2020-13754/qemu as no-dsa/intrusive for Stretch and Jessie.
- Mark CVE-2020-12829/qemu as no-dsa for Jessie.
- Mark CVE-2020-10756/qemu as not-affected for Jessie.
- Mark CVE-2020-13253/qemu as postponed for Jessie.
- Drop squirrelmail and xen for Stretch LTS.
- Add notes for tomcat8, shiro, and cacti to take care of the Stretch issues.
- Emailed team@security.d.o and debian-lts@l.d.o regarding possible clashes.
- Maintenance of LTS Survey on the self-hosted LimeSurvey instance. Received 1765 (just wow!) responses.
- Attended the fourth LTS meeting. MOM [here](http://meetbot.debian.net/debian-lts/2020/debian-lts.2020-07-30-14.59.html).
- General discussion on LTS private and [public mailing list](https://lists.debian.org/debian-lts/2020/07/threads.html).

---

## Other(s)
{{< figure src="/images/computing.jpg" >}}

Sometimes it gets hard to categorize work/things into a particular category.  
That's why I am writing all of those things inside this category.  
This includes two sub-categories and they are as follows.

#### Personal:

This month I did the following things:

- Released v0.2.0 of `rubocop-packaging` on [RubyGems](https://rubygems.org/gems/rubocop-packaging)! 💯  
  It's open-sourced and the repository is [here](https://github.com/utkarsh2102/rubocop-packaging).  
  Bug reports and pull requests are welcomed! 😉
- Released v0.1.0 of `get_root` on [RubyGems](https://rubygems.org/gems/get_root)! 💖  
  It's open-sourced and the repository is [here](https://github.com/utkarsh2102/get_root).
- Wrote [max-word-frequency](https://github.com/utkarsh2102/max_word_frequency), my Rails C1M2 programming assignment.  
  And made it pretty neater & cleaner!
- Refactored my `lts-dla` and `elts-ela` scripts entirely and wrote them in Ruby so that there are no issues and no false-positives! 🚀  
  Check [lts-dla here](https://github.com/utkarsh2102/utsh/commit/632ad0c0a6216bb0e5b35fde2a2379a97616dc19) and [elts-ela here](https://github.com/utkarsh2102/utsh/commit/614f13183075206596355fe315df0db7a6ec36fa).
- And finally, built my first Rails (mini) web-application! 🤗  
  The repository is [here](https://github.com/utkarsh2102/recipe_hunter). This was also a programming assignment (C1M3).  
  And furthermore, hosted it at [Heroku](https://recipe-hunter-2102.herokuapp.com/).


#### Open Source:

Again, this contains all the things that I couldn't categorize earlier.  
Opened several issues and PRs:

- [Issue #8273](https://github.com/rubocop-hq/rubocop/issues/8273) against [rubocop](https://github.com/rubocop-hq/rubocop), reporting a false-positive auto-correct for `Style/WhileUntilModifier`.
- [Issue #615](https://github.com/httprb/http/issues/615) against [http](https://github.com/httprb/http) reporting a weird behavior of a flaky test.
- [PR #3791](https://github.com/rubygems/rubygems/pull/3791) for [rubygems/bundler](https://github.com/rubygems/rubygems) to remove redundant `bundler/setup` require call from `spec_helper` generated by `bundle gem`.
- [Issue #3831](https://github.com/rubygems/rubygems/issues/3831) against [rubygems](https://github.com/rubygems/rubygems), reporting a traceback of undefined method, `rubyforge_project=`.
- [Issue #238](https://github.com/Nheko-Reborn/nheko/issues/238) against [nheko](https://github.com/Nheko-Reborn/nheko) asking for enhancement in showing the font name in the very font itself.
- [PR #2307](https://github.com/puma/puma/pull/2307) for [puma](https://github.com/puma/puma) to constrain `rake-compiler` to v0.9.4.
- And finally, I joined the [Cucumber](https://github.com/cucumber) organization! \o/

---

Thank you for sticking along for so long :)  

Until next time.  
`:wq` for today.
