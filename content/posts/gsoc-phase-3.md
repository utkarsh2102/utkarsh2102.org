+++
date = "2020-08-15 11:11:11 +0530"
title = "GSoC Phase 3"
slug = "gsoc-phase-3"
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
student for [Debian](https://www.debian.org/) to work on a project which is to write a linter
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
The previously written blogs can be found here:  
- [GSoC Phase 1 (part 1)](https://utkarsh2102.com/posts/gsoc-phase-1/).
- [GSoC Phase 1 (part 2)](https://utkarsh2102.com/posts/foss-in-june-20/).
- [GSoC Phase 2 (part 1)](https://utkarsh2102.com/posts/gsoc-phase-2/).
- [GSoC Phase 2 (part 2)](https://utkarsh2102.com/posts/foss-in-july-20/).
- And this is GSoC Phase 3 (part 1).

Whilst the daily updates are available at the above site^, I'll breakdown the important
parts here:

- Well, since the last 15 days, there hasn't been any significant change, mostly because
  I didn't get a lot of time to work on it. This is the DebConf20 month! \o/  
  Hear, hear, DebConf20 is here! 💖

- First of all, what I worked on was creating my DebConf20 talk, presenting this project that
  I am working on for the "GSoC 2020 Projects" session, proposed by the Outreach team.  
  Honestly, this was the hardest thing to do, really! Recording yourself is very hard.  
  It's almost equivalent to naming things and invalidating caches.

- After 7 or so unsuccessful tries, I finally could come up with something sane!  
  It still needed some work (lots of "umm"s) but I had given up on it, so I let it be.
  So I hope to see you see me at the session? :)  
  In any case, slides of my presentation can be found [here](https://slides.com/utkarsh2102/gsoc-dc20).

- Besides this, I've been helping in organizing DC20. Mostly the content team. And
  other things, here and there!

- Anyway, getting back to the project, I refactored the `generate_cops_documentation` task
  by using the newly added `CopsDocumentationGenerator` class in the RuboCop's source.

- I also started working on fixing the false-positives, which I mentioned in my last blog.  
  Hopefully with that, we'll be ready with another release!

- Besides, I've started working on the [Packaging Style Guide](https://packaging.rubystyle.guide),
  which documents all the reasoning behind this extension and the cops.

To conclude, I think in the next week or so, I'll be completing almost everything, from fixing
the pending bugs to adding 2 news cops and finally documenting the entire thing to the best
of my ability! \o/

---

Until next time.  
`:wq` for today.
