+++
date = "2023-03-30 11:11:11 +0530"
title = "FOSS Activites in March 2023"
slug = "foss-in-march-23"
images = [
    "/images/debian-logo-small.png",
    "/images/ubuntu-logo-small.png",
    "/images/debian-lts-small.png",
]
tags = [
    "debian",
    "ubuntu",
    "monthly",
]
categories = [
    "debian",
    "ubuntu",
    "open-source",
]
+++

Here's my (forty-second) monthly but brief update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 51st month of actively contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March 2019 and a [DD](https://wiki.debian.org/DebianDeveloper) on Christmas '19! \o/

There's a bunch of things I do, both, technical and non-technical. Here are the things I did this month:

- Looked for some Release team bits.
- Mentoring for newcomers.
- Ruby sprints remaining stuff.
- Bug work (on BTS and #debian-ruby) for rails and redmine.
- Moderation of -project mailing list.
- Reviewing Stefano's branch for DebConf prep.
- And finally, starting to do DebConf Bursary team setup.

A huge thanks to Freexian for sponsoring my Debian work and Entrouvert for sponsoring the Redmine backports. :D

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

This was my 26th month of actively contributing to [Ubuntu](https://ubuntu.com/about).
Now that I joined [Canonical to work on Ubuntu full-time](https://utkarsh2102.org/posts/hello-canonical/), there's a bunch of things I do! \o/

I mostly worked on different things, I guess.

I was too lazy to maintain a list of things I worked on so there's
no concrete list atm. Maybe I'll get back to this section later or
will start to list stuff from the fall, as I was doing before. :D

---

## Debian (E)LTS
{{< figure src="/images/debian-lts-small.png" >}}

[Debian Long Term Support (LTS)](https://www.freexian.com/en/services/debian-lts.html) is a project to extend the lifetime of all Debian stable releases to (at least) 5 years. Debian LTS is not handled by the Debian security team, but by a separate group of volunteers and companies interested in making it a success.  

And [Debian Extended LTS (ELTS)](https://deb.freexian.com/extended-lts) is its sister project, extending support to the stretch and jessie release (+2 years after LTS support).

This was my forty-second month as a Debian LTS and thirty-third month as a Debian ELTS paid contributor.  
I worked for 11.00 hours for LTS and 5.5 hours for ELTS.

#### LTS CVE Fixes and Announcements:

- Helped Scarlett with their uploads.
- Assisted Daniel with their RFA and pointed to a particular situation with ruby-roofah <-> ruby-rails-html-sanitize.
- Worked on ruby-rails-html-sanitize and added notes to the security-tracker.  
  TL;DR: we need newer methods in ruby-loofah to make the patches for ruby-rails-html-sanitize backportable.
- LTS traige.

#### ELTS CVE Fixes and Announcements:

- Helped and review ELTS documentation.
- ELTS triage.
- Lesser work on packages this month.

#### Other (E)LTS Work:

- Triaged [ruby-loofah](https://tracker.debian.org/pkg/ruby-loofah),
[ruby-sinatra](https://tracker.debian.org/pkg/ruby-sinatra),
[phpmyadmin](https://tracker.debian.org/pkg/phpmyadmin),
[ruby-rails-html-sanitizer](https://tracker.debian.org/pkg/ruby-rails-html-sanitizer),
[hdf5](https://tracker.debian.org/pkg/hdf5),
[cairosvg](https://tracker.debian.org/pkg/cairosvg),
[debian-goodies](https://tracker.debian.org/pkg/debian-goodies),
[sudo](https://tracker.debian.org/pkg/sudo),
[vim](https://tracker.debian.org/pkg/vim),
[openssh](https://tracker.debian.org/pkg/openssh),
[tidy-html5](https://tracker.debian.org/pkg/tidy-html5), and
[wireshark](https://tracker.debian.org/pkg/wireshark).
- Marked CVE-2023-27635/debian-goodies as no-dsa for stretch and jessie.
- Marked CVE-2023-2848{6,7}/sudo as no-dsa for buster and stretch and jessie.
- Marked CVE-2023-1175/vim as no-dsa for buster and stretch and jessie.
- Marked CVE-2023-28531/openssh as not-affected for stretch and jessie.
- Marked CVE-2021-33391/tidy-html5 as no-dsa for buster and stretch.
- Marked CVE-2023-1161/wireshark as no-dsa for buster and stretch.
- Auto EOL'd chromium, node-sqlite3, linux, firefox-esr, thunderbird, libde265, flatpak, stellarium, gpac, and liblouis.
- Helped and assisted new contributors joining Freexian (LTS/ELTS/internally).
- Answered questions (& discussions) on IRC (#debian-lts and #debian-elts) and Matrix.
- Participated and helped fellow members with their queries via private mail and chat.
- General and other discussions on LTS private and [public mailing list](https://lists.debian.org/debian-lts/2023/03/threads.html).
- Attended the monthly LTS meeting.

---

Until next time.  
`:wq` for today.
