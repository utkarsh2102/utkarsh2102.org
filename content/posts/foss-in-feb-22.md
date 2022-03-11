+++
date = "2022-03-01 11:11:11 +0530"
title = "FOSS Activites in February 2022"
slug = "foss-in-feb-22"
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

Here's my (twenty-ninth) monthly but brief update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 38th month of actively contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March 2019 and a [DD](https://wiki.debian.org/DebianDeveloper) on Christmas '19! \o/

I had been sick this month, so most of the time I spent away from system, recovering, et al,
and also went through the huge backlog that I had, which is starting to get smaller. :D

Anyway, I did the following stuff in Debian:

#### Uploads and bug fixes:

- [at](https://tracker.debian.org/pkg/at) (3.4.4-1) - Adding a DEP8 test for the package, fixing bug #985421.

#### Other $things:

- Mentoring for newcomers.
- Moderation of -project mailing list.

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

This was my 13th month of actively contributing to [Ubuntu](https://ubuntu.com/about).
Now that I joined [Canonical to work on Ubuntu full-time](https://utkarsh2102.com/posts/hello-canonical/), there's a bunch of things I do! \o/

I mostly worked on different things, I guess.

I was too lazy to maintain a list of things I worked on so there's
no concrete list atm. Maybe I'll get back to this section later or
will start to list stuff from the fall, as I was doing before. :D

---

## Debian (E)LTS
{{< figure src="/images/debian-lts-small.png" >}}

[Debian Long Term Support (LTS)](https://www.freexian.com/en/services/debian-lts.html) is a project to extend the lifetime of all Debian stable releases to (at least) 5 years. Debian LTS is not handled by the Debian security team, but by a separate group of volunteers and companies interested in making it a success.  

And [Debian Extended LTS (ELTS)](https://deb.freexian.com/extended-lts) is its sister project, extending support to the Jessie release (+2 years after LTS support).

This was my twenty-ninth month as a Debian LTS and eighteenth month as a Debian ELTS paid contributor.  
Whilst I was assigned 42.75 hours for LTS and 45.25 hours for ELTS, I could only work a little due to being sick and so
I spent 15.75 hours on LTS and 9.25 hours on ELTS and worked on the following things:  

#### LTS CVE Fixes and Announcements:

- Issued [DLA 2909-1](https://lists.debian.org/debian-lts-announce/2022/02/msg00003.html), fixing [CVE-2021-45079](https://security-tracker.debian.org/tracker/CVE-2021-45079), for [strongswan](https://tracker.debian.org/pkg/strongswan).  
  For Debian 9 stretch, these problems have been fixed in version 5.5.1-4+deb9u6.
- Issued [DLA 2912-1](https://lists.debian.org/debian-lts-announce/2022/02/msg00006.html), fixing [CVE-2021-3850](https://security-tracker.debian.org/tracker/CVE-2021-3850), for [libphp-adodb](https://tracker.debian.org/pkg/libphp-adodb).  
  For Debian 9 stretch, these problems have been fixed in version 5.20.9-1+deb9u1.
- Issued [DLA 2913-1](https://lists.debian.org/debian-lts-announce/2022/02/msg00007.html), fixing [CVE-2022-24130](https://security-tracker.debian.org/tracker/CVE-2022-24130), for [xterm](https://tracker.debian.org/pkg/xterm).  
  For Debian 9 stretch, these problems have been fixed in version 327-2+deb9u2.
- Issued [DLA 2918-1](https://lists.debian.org/debian-lts-announce/2022/02/msg00012.html), fixing [CVE-2021-20001](https://security-tracker.debian.org/tracker/CVE-2021-20001), for [debian-edu-config](https://tracker.debian.org/pkg/debian-edu-config).  
  For Debian 9 stretch, these problems have been fixed in version 1.929+deb9u5.
- Simultaneously, I've been working on the python* update but couldn't complete due to illness.

#### ELTS CVE Fixes and Announcements:

- Issued [ELA 559-1](https://deb.freexian.com/extended-lts/updates/ela-559-1-dojo/), fixing [CVE-2018-6561](https://security-tracker.debian.org/tracker/CVE-2018-6561), [CVE-2020-4051](https://security-tracker.debian.org/tracker/CVE-2020-4051), and [CVE-2021-23450](https://security-tracker.debian.org/tracker/CVE-2021-23450), for [dojo](https://tracker.debian.org/pkg/dojo).  
  For Debian 8 jessie, these problems have been fixed in version 1.10.2+dfsg-1+deb8u4.
- Issued [ELA 560-1](https://deb.freexian.com/extended-lts/updates/ela-560-1-libphp-adodb/), fixing [CVE-2021-3850](https://security-tracker.debian.org/tracker/CVE-2021-3850), for [libphp-adodb](https://tracker.debian.org/pkg/libphp-adodb).  
  For Debian 8 jessie, these problems have been fixed in version 5.15-1+deb8u2.
- Issued [ELA 561-1](https://deb.freexian.com/extended-lts/updates/ela-561-1-xterm/), fixing [CVE-2022-24130](https://security-tracker.debian.org/tracker/CVE-2022-24130), for [xterm](https://tracker.debian.org/pkg/xterm).  
  For Debian 8 jessie, these problems have been fixed in version 312-2+deb8u4.
- Also looking at python2.7 and python3.4 updates for jessie but couldn't complete due to illness.

#### Other (E)LTS Work:

- Triaged [xterm](https://tracker.debian.org/pkg/xterm),
[dojo](https://tracker.debian.org/pkg/dojo),
[strongswan](https://tracker.debian.org/pkg/strongswan),
[debian-edu-config](https://tracker.debian.org/pkg/debian-edu-config),
[libphp-adodb](https://tracker.debian.org/pkg/libphp-adodb), and
[libgit2](https://tracker.debian.org/pkg/libgit2),
- Read through the logs of the monthly Debian LTS meeting.
- Answered questions (& discussions) on IRC (#debian-lts and #debian-elts).
- General and other discussions on LTS private and [public mailing list](https://lists.debian.org/debian-lts/2022/02/threads.html).

#### Debian LTS Survey

I've spent 10 hours on the LTS survey on the following bits:  
(and 5 hours of the last month that I'm going to invoice this month)
- Put most of the content in the instance according to the question type.
- Been going back and forth updating the status of the survey on the issue.
- Trying to find a way to send to DDs - discussing with DPL, Raphael, and other people on the issue itself.
- Completing the last bits to start the survey for the paid contributors, at least. Talking to Jeremiah about this.

---

Until next time.  
`:wq` for today.
