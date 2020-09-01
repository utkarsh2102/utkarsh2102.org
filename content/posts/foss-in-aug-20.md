+++
date = "2020-09-02 23:30:00 +0530"
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

Until next time.  
`:wq` for today.
