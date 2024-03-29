+++
date = "2022-08-30 11:11:11 +0530"
title = "FOSS Activites in August 2022"
slug = "foss-in-aug-22"
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

Here's my (thirty-fifth) monthly but brief update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 44th month of actively contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March 2019 and a [DD](https://wiki.debian.org/DebianDeveloper) on Christmas '19! \o/

There's a bunch of things I do, both, technical and non-technical. Here are the things I did this month:

#### Debian Uploads

- [rails](https://tracker.debian.org/pkg/rails) (2:6.1.6.1+dfsg-1) - New upstream version, v6.1.6.1+dfsg to fix [CVE-2022-22577](https://security-tracker.debian.org/tracker/CVE-2022-22577), [CVE-2022-27777](https://security-tracker.debian.org/tracker/CVE-2022-27777), and [CVE-2022-32224](https://security-tracker.debian.org/tracker/CVE-2022-32224) and thereby, bug [#1011941](https://bugs.debian.org/1011941), [#1016982](https://bugs.debian.org/1016982), and [#1016140](https://bugs.debian.org/1016140).
- [python-pbcommand](https://tracker.debian.org/pkg/python-pbcommand) (2.1.1+git20220616.3f2e6c2-2) - Add python3-avro to Depends to fix autopkgtest.

#### Other $things:

- Being an AM for [Arun Kumar, process #1024](https://nm.debian.org/process/1024/).
- Sponsoring stuff for non-DDs.
- Mentoring for newcomers.
- Moderation of -project mailing list.

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

This was my 19th month of actively contributing to [Ubuntu](https://ubuntu.com/about).
Now that I joined [Canonical to work on Ubuntu full-time](https://utkarsh2102.org/posts/hello-canonical/), there's a bunch of things I do! \o/

I mostly worked on different things, I guess.

I was too lazy to maintain a list of things I worked on so there's
no concrete list atm. Maybe I'll get back to this section later or
will start to list stuff from the fall, as I was doing before. :D

---

## Debian (E)LTS
{{< figure src="/images/debian-lts-small.png" >}}

[Debian Long Term Support (LTS)](https://www.freexian.com/en/services/debian-lts.html) is a project to extend the lifetime of all Debian stable releases to (at least) 5 years. Debian LTS is not handled by the Debian security team, but by a separate group of volunteers and companies interested in making it a success.  

And [Debian Extended LTS (ELTS)](https://deb.freexian.com/extended-lts) is its sister project, extending support to the Jessie release (+2 years after LTS support).

This was my thirty-fifth month as a Debian LTS and twenty-sixth month as a Debian ELTS paid contributor.  
I worked for 14.00 hours for LTS and 19.00 hours for ELTS.

#### LTS CVE Fixes and Announcements:

- Issued [DLA 3094-1](https://lists.debian.org/debian-lts-announce/2022/09/msg00003.html), fixing [CVE-2021-0561](https://security-tracker.debian.org/tracker/CVE-2021-0561), for [flac](https://tracker.debian.org/pkg/flac).  
  For Debian 10 buster, these problems have been fixed in version 1.3.2-3+deb10u2.
- Issued [DLA 3095-1](https://lists.debian.org/debian-lts-announce/2022/09/msg00004.html), fixing [CVE-2022-30122](https://security-tracker.debian.org/tracker/CVE-2022-30122) and [CVE-2022-30123](https://security-tracker.debian.org/tracker/CVE-2022-30123), for [ruby-rack](https://tracker.debian.org/pkg/ruby-rack).  
  For Debian 10 buster, these problems have been fixed in version 2.0.6-3+deb10u1.
- Uploaded [rails/2:6.1.6.1+dfsg-1](https://tracker.debian.org/news/1356946/accepted-rails-26161dfsg-1-source-into-unstable/) to unstable for fixing [CVE-2022-22577](https://security-tracker.debian.org/tracker/CVE-2022-22577), [CVE-2022-27777](https://security-tracker.debian.org/tracker/CVE-2022-27777), and [CVE-2022-32224](https://security-tracker.debian.org/tracker/CVE-2022-32224) and thereby, bug [#1011941](https://bugs.debian.org/1011941), [#1016982](https://bugs.debian.org/1016982), and [#1016140](https://bugs.debian.org/1016140).
- Also looked at src:samba and how Ubuntu is looking at it. It's a mess, really. And it's different for both, LTS and ELTS. Worse for LTS with 36 opened issues. :)

#### ELTS CVE Fixes and Announcements:

- Issued [ELA 671-1](https://www.freexian.com/lts/extended/updates/ela-671-1-ruby-tzinfo/), fixing [CVE-2022-31163](https://security-tracker.debian.org/tracker/CVE-2022-31163), for [ruby-tzinfo](https://tracker.debian.org/pkg/ruby-tzinfo).  
  For Debian 9 stretch, these problems have been fixed in version 1.2.2-2+deb9u1.
- Issued [ELA 672-1](https://www.freexian.com/lts/extended/updates/ela-672-1-grunt/), fixing [CVE-2022-0436](https://security-tracker.debian.org/tracker/CVE-2022-0436), for [grunt](https://tracker.debian.org/pkg/grunt).  
  For Debian 9 stretch, these problems have been fixed in version 1.0.1-5+deb9u2.
- Started to look at src:tiff again. There are a lot of open CVEs piled up now. Drafted some fixes but halted the process to look at src:tiff in buster first - which I'll do next month.  
  I might do the update in two cycles. But more on that later.
- Also looked at src:samba and how Ubuntu is looking at it. It's a mess, really. Probably should write to the list. :/

#### Other (E)LTS Work:

- Triaged [grunt](https://tracker.debian.org/pkg/grunt),
[flac](https://tracker.debian.org/pkg/flac),
[ruby-rack](https://tracker.debian.org/pkg/ruby-rack),
[ruby-tzinfo](https://tracker.debian.org/pkg/ruby-tzinfo), and
[mbedtls](https://tracker.debian.org/pkg/mbedtls).
- Helped and assisted new (and fellow) contributors joining Freexian (LTS/ELTS).
- Answered questions (& discussions) on IRC (#debian-lts and #debian-elts) and Matrix.
- General and other discussions on LTS private and [public mailing list](https://lists.debian.org/debian-lts/2022/08/threads.html).

---

Until next time.  
`:wq` for today.
