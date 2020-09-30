+++
date = "2020-10-01 03:00:00 +0530"
title = "FOSS Activites in September 2020"
slug = "foss-in-sept-20"
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
]
categories = [
    "debian",
    "open-source",
]
+++

Here's my (twelfth) monthly update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 21st month of contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March last year and a [DD](https://wiki.debian.org/DebianDeveloper) last Christmas! \o/

I've been busy with my undergraduation stuff but I still squeezed out some time for the regular Debian work.
Here are the following things I did in Debian this month:

#### Uploads and bug fixes:

- [rails](https://tracker.debian.org/pkg/rails) (2:6.0.3.3+dfsg-1) - Fixing [CVE-2020-15169](https://security-tracker.debian.org/tracker/CVE-2020-15169)/[bug #970040](https://bugs.debian.org/970040).
- [ruby-openid-connect](https://tracker.debian.org/pkg/ruby-openid-connect) (1.1.8-1) - New upstream version, v1.1.8.
- [ruby-mini-magick](https://tracker.debian.org/pkg/ruby-mini-magick) (4.10.1-1) - Fixing FTBFS, [bug #966936](https://bugs.debian.org/966936).
- [ruby-open-graph-reader](https://tracker.debian.org/pkg/ruby-open-graph-reader) (0.7.0+dfsg-1) - New upstream version, v0.7.0.
- [ruby-string-direction](https://tracker.debian.org/pkg/ruby-string-direction) (1.2.2-1) - New upstream version, v1.2.2.
- [ruby-jquery-rails](https://tracker.debian.org/pkg/ruby-jquery-rails) (4.3.5-1) - New upstream version, v4.3.5.
- [ruby-leaflet-rails](https://tracker.debian.org/pkg/ruby-leaflet-rails) (1.6.0+dfsg-1) - New upstream version, v1.6.0.
- [ruby-jquery-rails](https://tracker.debian.org/pkg/ruby-jquery-rails) (4.3.5-2) - Fixing FTBFS, [bug #956604](https://bugs.debian.org/956604).
- [ruby-rubocop-packaging](https://tracker.debian.org/pkg/ruby-rubocop-packaging) (0.5.0-1) - Add support for auto-correct.

#### Other $things:

- Attended the Debian Ruby team meeting. Logs [here](http://meetbot.debian.net/debian-ruby/2020/debian-ruby.2020-09-04-16.29.html).
- Mentoring for newcomers.
- FTP Trainee reviewing.
- Moderation of -project mailing list.
- Sponsored `trace-cmd` for Sudip, `ruby-asset-sync` for Nilesh, and `mariadb-mysql-kbs` for William.

---

## RuboCop::Packaging - Helping the Debian Ruby team! \o/
![](/images/debian_ruby.png#center)

This [Google Summer of Code](https://summerofcode.withgoogle.com/), I worked on writing a linter that could flag offenses for lines of code
that are very troublesome for Debian maintainers while trying to package and maintain Ruby libraries and applications!

Whilst the GSoC period is over, I've been working on improving that tool and have exteneded that linter to now "auto-correct" these offenses
by itself! \o/  
You can now just use the `-A` flag and you're done! Boom! The game changer!

Here's a quick demo for this feature:

![](/images/packaging_autocorrector.gif#gif)

A few quick updates on [RuboCop::Packaging](https://github.com/utkarsh2102/rubocop-packaging):
- Has 4 cops, solving 4 different issues.
- 3 of them support auto-correction. Just use the `-A` flag.
- 5 releases so far, latest being v0.5.0.
- GitHub Repository: https://github.com/utkarsh2102/rubocop-packaging/
- Release notes: https://github.com/utkarsh2102/rubocop-packaging/releases/
- Documentation: https://docs.rubocop.org/rubocop-packaging/
- Style guide: https://packaging.rubystyle.guide/
- Being used by over [55 projects](https://github.com/utkarsh2102/rubocop-packaging/network/dependents)! \o/

I've also spent a considerable amount of time in raising awareness about this and in more general sense, about downstream maintenance.  
As a result, I raised a bunch of PRs which got really good response. I got [all of the 20 PRs merged upstream](https://github.com/utkarsh2102?tab=overview&from=2020-09-01&to=2020-09-30),
fixing these issues.

---

Until next time.  
`:wq` for today.
