+++
date = "2020-05-30 09:30:00 +0530"
title = "FOSS Activites in May 2020"
slug = "foss-in-may-20"
images = [
    "/images/debian-logo-small.png",
    "/images/ruby-logo-small.png",
    "/images/debian-lts-small.png",
    "/images/vendetta.jpg"
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

Here's my (eighth) monthly update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This month marks my 15 months of contributing to [Debian](https://www.debian.org/).
And 6th month as a [DD](https://wiki.debian.org/DebianDeveloper)! \o/  

Whilst I love doing Debian stuff, I have started spending more time on the programming
side now. And I hope to keep it this for some time now.  
Of course, I'll keep doing the Debian stuff, but just lesser in amount.

Anyway, the following are the things I did in May.

#### Uploads:

- [ruby-aggregate](https://tracker.debian.org/pkg/ruby-aggregate) (0.2.3-1) - got patches merged upstream.  
- [ruby-whenever](https://tracker.debian.org/pkg/ruby-whenever) (1.0.0-1) - new upstream version + take over maintenance.  
- [polybar](https://tracker.debian.org/pkg/polybar) (3.4.3-1) - fix GCC 10 compilation.  
- [ruby-dbus](https://tracker.debian.org/pkg/ruby-dbus) (0.16.0-1) - new upstream version + fix FTBFS (temporarily).  
- [ruby-rack](https://tracker.debian.org/pkg/ruby-rack) (2.1.1-5) - use `Dir.entries` instead of `Dir[glob]`. Fixes [CVE-2020-8161](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2020-8161).  
- [ruby-espeak](https://tracker.debian.org/pkg/ruby-espeak) (1.0.4-2) - fix FTBFS ([#952587](https://bugs.debian.org/952587)).  
- [ruby-libnotify](https://tracker.debian.org/pkg/ruby-libnotify) (0.9.4-1) - NEW ([#961577](https://bugs.debian.org/961577)). Needed by [batalert](https://github.com/utkarsh2102/batalert).  
- [batalert](https://tracker.debian.org/pkg/batalert) (0.3.0-1) - NEW ([#961580](https://bugs.debian.org/961580)).  
- [golang-github-zyedidia-tcell](https://tracker.debian.org/pkg/golang-github-zyedidia-tcell) (1.4.5-1) - fix tcell ID for micro.  
- [micro](https://tracker.debian.org/pkg/micro) (2.0.4-1) - new release [features](https://github.com/zyedidia/micro/releases/tag/v2.0.4) + change in [build path](https://salsa.debian.org/go-team/packages/micro/-/commit/9b9c01a89177acb9629f385ec14293eee1a1cb0b).  

#### Other $things:

- Hosted Ruby team meeting. Logs [here](http://meetbot.debian.net/debian-ruby/2020/debian-ruby.2020-05-08-16.53.html).  
- Attended Debian Perl Sprints. Report [here](https://lists.debian.org/debian-perl/2020/05/msg00051.html).  
- Sponsored `git-repo-updater` and `mplcursors` for Sudip.  
- Mentoring for newcomers.  
- FTP Trainee reviewing.  
- Moderation of -project mailing list.  
- Got selected for [GSoC'20 for Debian](https://bits.debian.org/2020/05/welcome-gsoc2020-interns.html)!

---

## Experimenting and improving Ruby libraries FTW!
{{< figure src="/images/ruby-logo-small.png" >}}

I have been very heavily involved with the [Debian Ruby team](https://wiki.debian.org/Teams/Ruby/) for over an year now.  
Thanks to Antonio Terceiro (and GSoC), I've started experimenting and taking more
interest in upstream development and improvement of these libraries.

This has the sole purpose of learning. It has gotten fun since I've started doing Ruby.  
And I hope it stays this way.

This month, I opened some issues and proposed a few pull requests. They are:

- [Issue #802](https://github.com/javan/whenever/issues/802) against `whenever` for Ruby2.7 test failures.
- [Issue #8](https://github.com/josephruscio/aggregate/issues/8) against `aggregate` asking upstream for a release on rubygems.
- [Issue #104](https://github.com/ruby/irb/issues/104) against `irb` for asking more about `Array.join("\n")`.
- [Issue #1391](https://github.com/mikel/mail/issues/1391) against `mail` asking upstream to cut a new release.
- [Issue #1655](https://github.com/rack/rack/issues/1655) against `rack` reporting test failures in the CVE fix.
- [Issue #84](https://github.com/mvidner/ruby-dbus/issues/84) against `ruby-dbus` for help with Debian bug [#836296](https://bugs.debian.org/836296).
- [Issue #85](https://github.com/mvidner/ruby-dbus/issues/85) against `ruby-dbus` asking if they still use `rDoc` for doc generation.
- [PR #9](https://github.com/josephruscio/aggregate/pull/9) against `aggregate` for dropping git from `gemspec`.
- [PR #804](https://github.com/javan/whenever/pull/804) against `whenever` for dropping git from `gemspec`.
- Packaged [ruby-cmath](https://tracker.debian.org/pkg/ruby-cmath) as it was split from Ruby2.7; cf: ([#961213](https://bugs.debian.org/961213)).

---

## Debian LTS
{{< figure src="/images/debian-lts-small.png" >}}

Debian Long Term Support (LTS) is a project to extend the lifetime of all Debian stable releases
to (at least) 5 years. Debian LTS is not handled by the Debian security team, but by a separate group
of volunteers and companies interested in making it a success.  

This was my eighth month as a Debian LTS paid contributor. I was assigned 17.25 hours and worked on
the following things:  

#### CVE Fixes and Announcements:

- Issued [DLA 2191-1](https://lists.debian.org/debian-lts-announce/2020/04/msg00029.html), fixing [CVE-2020-10683](https://security-tracker.debian.org/tracker/CVE-2020-10683), for [dom4j](https://tracker.debian.org/dom4j).  
  For Debian 8 "Jessie", this problem has been fixed in version 1.6.1+dfsg.3-2+deb8u2.  

- Issued [DLA 2192-1](https://lists.debian.org/debian-lts-announce/2020/04/msg00030.html), fixing [CVE-2020-10663](https://security-tracker.debian.org/tracker/CVE-2020-10663), for [ruby2.1](https://tracker.debian.org/ruby2.1).  
  For Debian 8 "Jessie", this problem has been fixed in version 2.1.5-2+deb8u10.  

- Issued [DLA 2208-1](https://lists.debian.org/debian-lts-announce/2020/05/msg00011.html), fixing [CVE-2020-11026](https://security-tracker.debian.org/tracker/CVE-2020-11026), [CVE-2020-11027](https://security-tracker.debian.org/tracker/CVE-2020-11027), [CVE-2020-11028](https://security-tracker.debian.org/tracker/CVE-2020-11028), and [CVE-2020-11029](https://security-tracker.debian.org/tracker/CVE-2020-11026), for [wordpress](https://tracker.debian.org/wordpress).  
  For Debian 8 "Jessie", these problems have been fixed in version 4.1.30+dfsg-0+deb8u1.  

- Issued [DLA 2210-1](https://lists.debian.org/debian-lts-announce/2020/05/msg00013.html), fixing [CVE-2020-3810](https://security-tracker.debian.org/tracker/CVE-2020-3810), for [apt](https://tracker.debian.org/apt).  
  This update was prepared by the maintainer, Julian. I just took care of the paperwork.  
  For Debian 8 "Jessie", this problem has been fixed in version 1.0.9.8.6.

#### Other LTS Work:

- Triaged [tika](https://tracker.debian.org/pkg/tika),
[freerdp](https://tracker.debian.org/pkg/freerdp), and
[apache2](https://tracker.debian.org/pkg/apache2).
- Mark CVE-2020-12105/openconnect as ~~no-dsa~~ not-affected for Jessie.
- Mark CVE-2020-9489/tika as ~~no-dsa~~ ignored for Jessie.
- Mark CVE-2020-11025/wordpres as not-affected for Jessie.
- Add fix for Add fix for CVE-2019-18823/condor.
- Requested CVE for [bug#60251](https://bz.apache.org/bugzilla/show_bug.cgi?id=60251) against [apache2](https://tracker.debian.org/pkg/apache2).
- Raised [issue #947](https://github.com/sympa-community/sympa/issues/947) against sympa reporting an incomplete patch for CVE-2020-10936.
- Created the LTS Survey on the self-hosted LimeSurvey instance.
- Attended the second LTS meeting. Logs [here](http://meetbot.debian.net/debian-lts/2020/debian-lts.2020-05-28-14.58.html).
- General discussion on LTS private and [public mailing list](https://lists.debian.org/debian-lts/2020/05/threads.html).

---

## Other(s)
{{< figure src="/images/vendetta.jpg" >}}

Sometimes it gets hard to categorize work/things into a particular category.  
That's why I am writing all of those things inside this category.  
This includes two sub-categories and they are as follows.

#### Personal:

This month I could get the following things done:

- Wrote and published my first Ruby gem/library/tool on [RubyGems](https://rubygems.org/gems/batalert)! 💯  
  It's open-sourced and the repository is [here](https://github.com/utkarsh2102/batalert).  
  Bug reports and pull requests are welcomed! 😉
- Wrote a small Ruby script (available [here](https://github.com/utkarsh2102/utsh/blob/master/gem-install.rb)) to install Ruby gems from Gemfile(.lock).  
  Needed this when I hit a bug while using [ruby-standalone](https://salsa.debian.org/ruby-team/ruby-standalone), which Antonio fixed pretty quickly! 🚀
- Had a coffee chat with John Coghlan! 🤗  
  Tweet [here](https://twitter.com/utkarsh2102/status/1266342128130461696).

#### Open Source:

Again, this contains all the things that I couldn't categorize earlier.  
Opened several issues and did a PR review:

- [Issue #15434](https://github.com/ariya/phantomjs/issues/15434) against `phantomjs`, asking to look into CVE-2019-17221. Still no action :/
- [Issue #947](https://github.com/sympa-community/sympa/issues/947) against `sympa`, reporting an incomplete patch for CVE-2020-10936.
- [Issue #2102](https://github.com/polybar/polybar/issues/2102) against `polybar`, mentioning that the build is not reproducible.
- [Issue #5521](https://github.com/libgit2/libgit2/issues/5521) against `libgit2`, mentioning that the build is not reproducible.
- Reviewed [PR #5523](https://github.com/libgit2/libgit2/pull/5523) for `polybar`, which was a fix for the above issue.

---

Until next time.  
`:wq` for today.
