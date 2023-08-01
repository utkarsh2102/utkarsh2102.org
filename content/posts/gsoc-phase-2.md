+++
date = "2020-07-15 11:11:11 +0530"
title = "GSoC Phase 2"
slug = "gsoc-phase-2"
tags = [
    "debian",
    "gsoc"
]
images = ["/images/debian_ruby.png"]
categories = [
    "debian",
    "open-source",
]
+++

Hello,

In early May, I got selected as a [Google Summer of Code](https://summerofcode.withgoogle.com/)
student for [Debian](https://www.debian.org/) to work on a  project which is to write a linter
(an extension to [RuboCop](https://rubocop.org/)).  
This tool is mostly to help the [Debian Ruby team](https://wiki.debian.org/Teams/Ruby/).
And that is the best part, I love working in/for/with the Ruby team!  
(I've been an active part of the team for 19 months now :))

![](/images/debian_ruby.png#center)


More details about the project can be found [here, on the wiki](https://wiki.debian.org/SummerOfCode2020/Projects/#SummerOfCode2020.2FApprovedProjects.2FUpstreamDownstreamCooperationInRuby.Upstream.2FDownstream_cooperation_in_Ruby).  
And also, I have got the best mentors I could've possibly asked for: [Antonio Terceiro](https://github.com/terceiro)
and [David Rodríguez](https://github.com/deivid-rodriguez/) 💖


So, the program began on 1st June and I've been working since then. I log my daily updates at
[gsocwithutkarsh2102.tk](https://gsocwithutkarsh2102.tk/).  
The blog for the first part of phase 1 can be found [here](https://utkarsh2102.org/posts/gsoc-phase-1/)
and that of second part of phase 1 can be found [here](https://utkarsh2102.org/posts/foss-in-june-20/).

Whilst the daily updates are available at the above site^, I'll breakdown the important
parts here:

- After the, what I'd like to call, successful Phase 1, whilst using this extension on
  GitLab's [omnibus-gitlab](https://gitlab.com/gitlab-org/omnibus-gitlab/) repository,
  I discovered a bug (as reported via [issue #5](https://github.com/utkarsh2102/rubocop-packaging/issues/5)),
  which basically threw the following error:
  > An error occurred while Packaging/GemspecGit cop was inspecting
    /home/utkarsh/github/omnibus-gitlab/files/gitlab-cookbooks/gitlab/recipes/bootstrap_disable.rb.  
  > To see the complete backtrace run rubocop -d.

  ...which was not good.

- This bug was a false-negative and the fix turned out to be simple, which was raised via
  [PR #6](https://github.com/utkarsh2102/rubocop-packaging/pull/6).  
  Since the extension was now working fine against omnibus-gitlab (which is...quite huge!),
  I rolled out a [v0.1.1 release](https://github.com/utkarsh2102/rubocop-packaging/releases/tag/v0.1.1)! 🎉

- Next, I implemented the 2nd cop, fixing `require` and `require_relative` calls which map from
  `spec(s)/test(s)` to the `lib` directory.  
  This was raised via a [WIP PR #4](https://github.com/utkarsh2102/rubocop-packaging/pull/4).

- We had our meeting where we discussed that it would rather make sense to split these cops into
  two parts and also, thanks to David's [elaborative comment](https://github.com/utkarsh2102/rubocop-packaging/pull/4#issuecomment-648646511)
  on the situation.  
  With this, we decided to split the cops into two.

- Then I worked on:
  - Splitting the cops via commit [@6765fec8](https://github.com/utkarsh2102/rubocop-packaging/pull/4/commits/6765fec8bf3326dc0fb2f4647f06c1d91a861d55).
  - Dropping Ruby2.4 support via commit [@3681e9a3](https://github.com/utkarsh2102/rubocop-packaging/pull/4/commits/3681e9a3e178bc3eee081a4c98f7f68019b506c3).
  - Diversifying tests via commit [@335a14e2](https://github.com/utkarsh2102/rubocop-packaging/pull/4/commits/335a14e29deda41f8878ccd50abdd2a6beae8950).

- At this point, we hit yet another obstacle. Correctly determining the root directory of a project
  at runtime. This is...tricky. Not impossible (of course) but tricky.  
  So my "homework" was to find such a thing that does that by default.

- For the next 4 days, I tried to find something that could do this bit. But unfortunately, I
  couldn't.  
  So I wrote one myself. I wrote [get_root](https://github.com/utkarsh2102/get_root), which solves this
  problem.  
  The only thing that one needs to take care while using `get_root` is that it has to be a `git`
  repository. That's a...trade-off.

- In the next meeting, we discussed that this is a bit of an overkill. `get_root` should've been
  written as a helper function and not as another library, which David and Antonio pointed out
  correctly. But it was already too late :P  
  I had already made a [v 0.1.0 release](https://rubygems.org/gems/get_root).  
  (So in case you're a Rubyist and want to find the root directory of a git repository, consider using
  this :P)  
  Besides, Antonio also pointed out that it should take another arguement as to from point from where
  the file is being inspected. Hm, unsure how to do that..

- Meanwhile, I exported `get_root` as a helper function, David solved all the problem altogether at
  once via [rubocop's PR #8314](https://github.com/rubocop-hq/rubocop/pull/8314).  
  This introduced a new (public) method `#project_root` which superseeded `get_root` and one could
  now get the root directory via `RuboCop::ConfigLoader.project_root`. Ain't he amazing!? \o/

- This also means, I reverted those changes altogether and tweaked my WIP PR to inculcate these
  changes via commit [@b06a8f86](https://github.com/utkarsh2102/rubocop-packaging/pull/4/commits/b06a8f86836db03dd9d3f56dffab7daa6d09f7b9).  
  However, the specs fail. But that doesn't mean that the changes aren't correct :P  
  They are pretty much right and working fine. To make that sure, I locally installed this library
  and used on other projects to make sure that it indeed is working alright, as it should! \o/

- And here I am on the 15th day :)


Well, the best part yet?  
`rubocop-packaging` is being used by [batalert](https://rubygems.org/gems/batalert), [arbre](https://rubygems.org/gems/arbre),
[rspec-stubbed_env](https://rubygems.org/gems/rspec-stubbed_env), [rspec-pending_for](https://rubygems.org/gems/rspec-pending_for),
[ISO8601](https://rubygems.org/gems/ISO8601), [get_root](https://rubygems.org/gems/get_root) (😛),
[gir_ffi](https://rubygems.org/gems/gir_ffi), [linter](https://rubygems.org/gems/linter), and
[cucumber-rails](https://rubygems.org/gems/cucumber-rails).

Whilst it has been a lot of fun so far, my plate has started to almost...overflow. It seems that I've
got a lot of things to work on (and already things that are due!).  
From my major project, college *stuff to my GSoC project, Debian (E)LTS, and a lot *more.

Thanks to Antonio for helping me out with *other things (which maps back to his sayings in Paris \o/).

---

Until next time.  
`:wq` for today.
