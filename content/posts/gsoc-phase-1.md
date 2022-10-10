+++
date = "2020-06-15 11:11:11 +0530"
title = "GSoC Phase 1"
slug = "gsoc-phase-1"
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

Earlier last month, I got selected as a [Google Summer of Code](https://summerofcode.withgoogle.com/)
student for [Debian](https://www.debian.org/) again! \o/  
And as [Chandler](https://www.youtube.com/watch?v=iqyBtWIZTkI) would say,
> Could I be any more happier?


Well, this time, my project is basically to write a linter (an extension to [RuboCop](https://rubocop.org/)).
This tool is mostly to help the [Debian Ruby team](https://wiki.debian.org/Teams/Ruby/).
And that is the best part, I love working in/for/with the Ruby team!  
(I've been an active part of the team for 18 months now :))

![](/images/debian_ruby.png#center)


More details about the project can be found [here, on the wiki](https://wiki.debian.org/SummerOfCode2020/Projects/#SummerOfCode2020.2FApprovedProjects.2FUpstreamDownstreamCooperationInRuby.Upstream.2FDownstream_cooperation_in_Ruby).  
And also, I have got the best mentors I could've possibly asked for: [Antonio Terceiro](https://github.com/terceiro)
and [David Rodríguez](https://github.com/deivid-rodriguez/) 💖


So, the program began on 1st June and I've been working since then. I log my daily updates at
[gsocwithutkarsh2102.tk](https://gsocwithutkarsh2102.tk/).

Whilst the daily updates are available at the above site^, I'll breakdown the important
parts here:

- During the first three days, I looked for a potential solution to the usage of
  `git ls-files` in the gemspec files. This has been the most problematic thing for us.
  - Apart from the option of using `Dir` or `Dir.glob`, the best (closest) possible solution
    (right now) is to use `Rake::FileList` which tries to respects the `.gitignore` file.
  - I stumbled upon this interesting gem, [fast_ignore](https://github.com/robotdana/fast_ignore).
    It is the *exact* thing which we want to use but unfortunately, to use it inside other
    gemspec files, it should be vendored inside [bundler's](https://rubygems.org/gems/bundler)
    code.

- We had our [first meeting](https://gsocwithutkarsh2102.tk/log/2020/06/04/day4.html) on the
  fourth day and we decided to hold meetings every Thursday for the next 12 weeks.

- For the next five days, I learned more of Ruby and figured out what to do and how to do it.  
  If you'd like to know what exactly I did in these 5 days, I'd suggest you to read the daily
  logs for those respective days.

- During the next to two days, the first part of the project, the GemspecGit Cop, was
  implemented.  
  This cop will correctly determine the usage of "git" in the gemspec files and would tell
  the developers and the maintainers to replace them with pure Ruby alternatives with giving
  them a proper reason to do so. Much thanks to [Dana](https://github.com/robotdana/) for her
  help -- she took out time to pair-program with me! 💖

- We had our [second weekly meeting](https://gsocwithutkarsh2102.tk/log/2020/06/11/day11.html)
  where I finally told Antonio and David that the first part is already done (\o/) and we
  discussed some things and even pair-programmed :D

- I took the weekend off (and something terrible happened) but anyways, I managed to get
  together some time and energy to document the source code and raised this
  [PR #2](https://github.com/utkarsh2102/rubocop-packaging/pull/2/).

- And here I am on the 15th day :)


It has been a lot of fun so far! Though I am little worried on how to implement the next part
of the project as I am not sure how to check only a particalar directory for some relative
require calls.  
But I think, that's okay, somehow, something will work out. And I can always ask around
others and check other cops to see how it's done! ¯\\_(ツ)_/¯

---

Until next time.  
`:wq` for today.
