+++
date = "2020-09-30 04:30:00 +0530"
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

Whilst the GSoC period is over, I've been working on improving that tool and have extended that linter to now "auto-correct" these offenses
by itself! \o/  
You can now just use the `-A` flag and you're done! Boom! The ultimate game-changer!

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

## Debian (E)LTS
{{< figure src="/images/debian-lts-small.png" >}}

[Debian Long Term Support (LTS)](https://www.freexian.com/en/services/debian-lts.html) is a project to extend the lifetime of all Debian stable releases to (at least) 5 years. Debian LTS is not handled by the Debian security team, but by a separate group of volunteers and companies interested in making it a success.  

And [Debian Extended LTS (ELTS)](https://deb.freexian.com/extended-lts) is its sister project, extending support to the Jessie release (+2 years after LTS support).

This was my twelfth month as a Debian LTS and third month as a Debian ELTS paid contributor.  
I was assigned 19.75 hours for LTS and 15.00 hours for ELTS and worked on the following things:  
(for LTS, I over-worked for 11 hours last month on the survey so only had 8.75 hours this month!)

#### LTS CVE Fixes and Announcements:

- Issued [DLA 2362-1](https://lists.debian.org/debian-lts-announce/2020/09/msg00001.html), fixing [CVE-2020-11984](https://security-tracker.debian.org/tracker/CVE-2020-11984), for [uwsgi](https://tracker.debian.org/pkg/uwsgi).  
  For Debian 9 Stretch, these problems have been fixed in version 2.0.14+20161117-3+deb9u3.
- Issued [DLA 2363-1](https://lists.debian.org/debian-lts-announce/2020/09/msg00002.html), fixing [CVE-2020-17446](https://security-tracker.debian.org/tracker/CVE-2020-17446), for [asyncpg](https://tracker.debian.org/pkg/asyncpg).  
  For Debian 9 Stretch, these problems have been fixed in version 0.8.4-1+deb9u1.
- Started working on [ruby-kaminari](https://tracker.debian.org/pkg/ruby-kaminari), [ruby-rack-cors](https://tracker.debian.org/pkg/ruby-rack-cors), and [ruby-json-jwt](https://tracker.debian.org/pkg/ruby-json-jwt).

#### ELTS CVE Fixes and Announcements:

- Issued [ELA 274-1](https://deb.freexian.com/extended-lts/updates/ela-274-1-uwsgi), fixing [CVE-2020-11984](https://security-tracker.debian.org/tracker/CVE-2020-11984), for [uwsgi](https://tracker.debian.org/pkg/uwsgi).  
  For Debian 8 Jessie, these problems have been fixed in version 2.0.7-1+deb8u3.
- Issued [ELA 275-1](https://deb.freexian.com/extended-lts/updates/ela-275-1-libx11), fixing [CVE-2020-14363](https://security-tracker.debian.org/tracker/CVE-2020-14363), for [libx11](https://tracker.debian.org/pkg/libx11).  
  For Debian 8 Jessie, these problems have been fixed in version 2:1.6.2-3+deb8u4.
- Issued [ELA 278-1](https://deb.freexian.com/extended-lts/updates/ela-278-1-ruby-rack), fixing [CVE-2020-8184](https://security-tracker.debian.org/tracker/CVE-2020-8184), for [ruby-rack](https://tracker.debian.org/pkg/ruby-rack).  
  For Debian 8 Jessie, these problems have been fixed in version 1.5.2-3+deb8u4.
- Also worked on updating the version of [clamAV](https://tracker.debian.org/pkg/clamav) from v0.101.5 to v0.102.4.  
  This was a bit tricky package to work on since it involved an ABI/API change and was more or less a transition.
  Super thanks to Emilio for his invaluable help and him taking over the package, finishing, and uploading it in the end.

#### Other (E)LTS Work:

- Front-desk duty from 31-08 to 06-09 and from 28-09 onward for both LTS and ELTS.
- Triaged [apache2](https://tracker.debian.org/pkg/apache2),
[cryptsetup](https://tracker.debian.org/pkg/cryptsetup),
[nasm](https://tracker.debian.org/pkg/nasm),
[node-bl](https://tracker.debian.org/pkg/node-bl),
[plinth](https://tracker.debian.org/pkg/plinth),
[qemu](https://tracker.debian.org/pkg/qemu),
[rsync](https://tracker.debian.org/pkg/rsync),
[ruby-doorkeeper](https://tracker.debian.org/pkg/ruby-doorkeeper), and
[uwsgi](https://tracker.debian.org/pkg/uwsgi).
- Marked CVE-2020-15094/symfony as not-affected for Stretch.
- Marked CVE-2020-{9490,11993}/apache2 as ignored for Stretch.
- Marked CVE-2020-8244/node-bl as no-dsa for Stretch.
- Marked CVE-2020-24978/nasm as no-dsa for Stretch.
- Marked CVE-2020-25073/plinth as no-dsa for Stretch.
- Marked CVE-2020-15094/symfony as not-affected for Jessie.
- Marked CVE-2020-14382/cryptsetup as not-affected for Jessie.
- Marked CVE-2020-14387/rsync as not-affected for Jessie.
- Auto EOL'ed ark, collabtive, linux, nasm, node-bl, and thunderbird for Jessie.
- Use `mktemp` instead of `tempfile` in `bin/auto-add-end-of-life.sh`.
- Attended the fifth LTS meeting. Logs [here](http://meetbot.debian.net/debian-lts/2020/debian-lts.2020-09-24-14.58.html).
- General discussion on LTS private and [public mailing list](https://lists.debian.org/debian-lts/2020/09/threads.html).

---

Until next time.  
`:wq` for today.
