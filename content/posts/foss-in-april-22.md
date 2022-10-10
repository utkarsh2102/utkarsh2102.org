+++
date = "2022-04-30 11:11:11 +0530"
title = "FOSS Activites in April 2022"
slug = "foss-in-april-22"
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

Here's my (thirty-first) monthly but brief update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 40th month of actively contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March 2019 and a [DD](https://wiki.debian.org/DebianDeveloper) on Christmas '19! \o/

There's a bunch of things I did this month but mostly non-technical, now that DC22 is around the corner. Here are the things I did:

#### Debian Uploads

- Helped Andrius w/ FTBFS for php-text-captcha, reported via #977403.
  - I fixed the samed in Ubuntu a couple of months ago and they copied over the patch here.

#### Other $things:

- Volunteering for DC22 Content team.
- Leading the Bursary team w/ Paulo.
- Answering a bunch of questions of referees and attendees around bursary.
- Being an AM for [Arun Kumar, process #1024](https://nm.debian.org/process/1024/).
- Mentoring for newcomers.
- Moderation of -project mailing list.

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

This was my 15th month of actively contributing to [Ubuntu](https://ubuntu.com/about).
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

This was my thirty-first month as a Debian LTS and twentieth month as a Debian ELTS paid contributor.  
I worked for 23.25 hours for LTS and 20.00 hours for ELTS.

#### LTS CVE Fixes and Announcements:

- Issued [DLA 2976-1](https://lists.debian.org/debian-lts-announce/2022/04/msg00007.html), fixing [CVE-2022-1271](https://security-tracker.debian.org/tracker/CVE-2022-1271), for [gzip](https://tracker.debian.org/pkg/gzip).  
  For Debian 9 stretch, these problems have been fixed in version 1.6-5+deb9u1.
- Issued [DLA 2977-1](https://lists.debian.org/debian-lts-announce/2022/04/msg00008.html), fixing [CVE-2022-1271](https://security-tracker.debian.org/tracker/CVE-2022-1271), for [xz-utils](https://tracker.debian.org/pkg/xz-utils).  
  For Debian 9 stretch, these problems have been fixed in version 5.2.2-1.2+deb9u1.
- Working on src:tiff and src:mbedtls to fix the issues, _still_ waiting for more issues to be reported, though.
- Looking at src:mutt CVEs. Haven't had the time to complete but shall roll out next month.

#### ELTS CVE Fixes and Announcements:

- Issued [ELA 593-1](https://deb.freexian.com/extended-lts/updates/ela-593-1-gzip/), fixing [CVE-2022-1271](https://security-tracker.debian.org/tracker/CVE-2022-1271), for [gzip](https://tracker.debian.org/pkg/gzip).  
  For Debian 8 jessie, these problems have been fixed in version 1.6-4+deb8u1.
- Issued [ELA 594-1](https://deb.freexian.com/extended-lts/updates/ela-594-1-xz-utils/), fixing [CVE-2022-1271](https://security-tracker.debian.org/tracker/CVE-2022-1271), for [xz-utils](https://tracker.debian.org/pkg/xz-utils).  
  For Debian 8 jessie, these problems have been fixed in version 5.1.1alpha+20120614-2+deb8u1.
- Issued [ELA 598-1](https://deb.freexian.com/extended-lts/updates/ela-598-1-python2.7/), fixing [CVE-2019-16935](https://security-tracker.debian.org/tracker/CVE-2019-16935), [CVE-2021-3177](https://security-tracker.debian.org/tracker/CVE-2021-3177), and [CVE-2021-4189](https://security-tracker.debian.org/tracker/CVE-2021-4189), for [python2.7](https://tracker.debian.org/pkg/python2.7).  
  For Debian 8 jessie, these problems have been fixed in version 2.7.9-2-ds1-1+deb8u9.
- Working on src:tiff and src:beep to fix the issues, _still_ waiting for more issues to be reported for src:tiff and src:beep is a bit of a PITA, though. :)

#### Other (E)LTS Work:

- Triaged [gzip](https://tracker.debian.org/pkg/gzip),
[xz-utils](https://tracker.debian.org/pkg/xz-utils),
[tiff](https://tracker.debian.org/pkg/tiff),
[beep](https://tracker.debian.org/pkg/beep),
[python2.7](https://tracker.debian.org/pkg/python2.7),
[python-django](https://tracker.debian.org/pkg/python-django), and
[libgit2](https://tracker.debian.org/pkg/libgit2),
- Signed up to be a Freexian Collaborator! \o/
- Read through some bits around that.
- Helped and assisted new contributors joining Freexian.
- Answered questions (& discussions) on IRC (#debian-lts and #debian-elts).
- General and other discussions on LTS private and [public mailing list](https://lists.debian.org/debian-lts/2022/04/threads.html).
- Attended monthly Debian meeting. Held on Jitsi this month.

#### Debian LTS Survey

I've spent 18 hours on the LTS survey on the following bits:  
- Rolled out the announcement. Started the survey.
- Answered a bunch of queries, people asked via e-mail.
- Looked at another bunch of tickets: https://salsa.debian.org/freexian-team/project-funding/-/issues/23.
- Sent a reminder and fixed a few things here and there.
- Gave a status update during the meeting.
- Extended the duration of the survey.

---

Until next time.  
`:wq` for today.
