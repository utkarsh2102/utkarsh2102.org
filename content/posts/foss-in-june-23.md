+++
date = "2023-06-30 11:11:11 +0530"
title = "FOSS Activites in June 2023"
slug = "foss-in-june-23"
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

Here's my (forty-fifth) monthly but brief update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 54th month of actively contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March 2019 and a [DD](https://wiki.debian.org/DebianDeveloper) on Christmas '19! \o/

There's a bunch of things I do, both, technical and non-technical. Here are the things I did this month:

### Uploads

- [ccextractor](https://tracker.debian.org/pkg/ccextractor) (0.94+ds1-2) - Fix FTBFS w/ FFmpeg 5.0 and Tesseract 5.0. ([debbug#1004581](https://bugs.debian.org/1004581))

### Others

- Moderation of -project mailing list.
- Mentoring for newcomers.
- Bursary team stuff - starting to analyze requests, gathering refs, and dry-running the scripts.

A huge thanks to Freexian for sponsoring my Debian work. :D

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

This was my 29th month of actively contributing to [Ubuntu](https://ubuntu.com/about).
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

This was my forty-fifth month as a Debian LTS and thirty-sixth month as a Debian ELTS paid contributor.  
I worked for 11.75 hours for LTS and 0.00 hours for ELTS.

#### LTS CVE Fixes and Announcements:

- Issued [DLA 3450-1](https://lists.debian.org/debian-lts-announce/2023/06/msg00012.html), fixing [CVE-2021-33621](https://security-tracker.debian.org/tracker/CVE-2021-33621) and [CVE-2022-28739](https://security-tracker.debian.org/tracker/CVE-2022-28739), for [ruby2.5](https://tracker.debian.org/pkg/ruby2.5).  
  For Debian 10 buster, these problems have been fixed in version 2.5.5-3+deb10u6.
- Replied to Roberto's mail for the ruby2.5 regression post-mortem.
- Prepared ruby-rack security update for the security team.
  - Some regressions reported in ruby-sinatra's autopkgtest. Investigating further.
- Started to prep ruby2.7 security update but paused that work in favor of investigating the regression above.

#### Other (E)LTS Work:

- Triaged [ruby-rack](https://tracker.debian.org/pkg/ruby-rack),
[ruby-sinatra](https://tracker.debian.org/pkg/ruby-sinatra),
[ruby2.5](https://tracker.debian.org/pkg/ruby2.5),
[ruby2.7](https://tracker.debian.org/pkg/ruby2.7).
- Helped and assisted fellow Freexian contributors (LTS/ELTS/internally).
- Answered questions (& discussions) on IRC (#debian-lts and #debian-elts) and Matrix.
- Participated and helped fellow members with their queries via private mail and chat.
- General and other discussions on LTS private and [public mailing list](https://lists.debian.org/debian-lts/2023/06/threads.html).
- Attended the monthly LTS meeting.

---

Until next time.  
`:wq` for today.
