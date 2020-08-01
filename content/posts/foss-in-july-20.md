+++
date = "2020-08-01 01:30:00 +0530"
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

- [Marc Andre](https://github.com/marcandre), very kindly, helped in [fixing the specs](https://github.com/marcandre/rubocop-packaging/commit/90d23d16dff4fd00652d3e5c7f32c88d9c987225) that were failing earlier this month. Well, the problem were the specs, but I am still confused how. Anyway..
- Finished documentation of the second cop and marked the PR as ready to be reviewed.
- David reviewed and suggested some really good changes and I fixed/tweaked that PR as per his suggestion to finally finish the last bits of the second cop, `RelativeRequireToLib`.
- Merged the PR upon two approvals and released it as v0.2.0! 💖
- We had our next weekly meeting where we discussed the next steps and the things that are supposed to be done for the next set of cops.
- Introduced [rubocop-packaging](https://github.com/utkarsh2102/rubocop-packaging) to the outer world and requested other upstream projects to use it! It is being used by [13 other projects](https://github.com/utkarsh2102/rubocop-packaging/network/dependents?package_id=UGFja2FnZS0xMjY1ODQyMzQ1) already! 😭💖
- Started to work on [packaging-style-guide](https://github.com/utkarsh2102/packaging-style-guide) but nothing really is pushed to the public repository.
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


Thank you for sticking along for so long :)  

Until next time.  
`:wq` for today.
