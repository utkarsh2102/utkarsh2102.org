+++
date = "2022-03-30 11:11:11 +0530"
title = "FOSS Activites in March 2022"
slug = "foss-in-march-22"
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

Here's my (thirtieth) monthly but brief update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 39th month of actively contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March 2019 and a [DD](https://wiki.debian.org/DebianDeveloper) on Christmas '19! \o/

I recovered this month and cleared up a bunch of my backlog. So a good month, that way.

I didn't do any uploads this month but I still did the following this month:

#### Other $things:

- Volunteering for DC22 Content team.
- Volunteering for DC22 Bursary team.
- Being a DC22 Bursary lead along w/ Paulo.
- Being an AM for [Arun Kumar, process #1024](https://nm.debian.org/process/1024/).
- Mentoring for newcomers.
- Moderation of -project mailing list.

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

This was my 14th month of actively contributing to [Ubuntu](https://ubuntu.com/about).
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

This was my thirtieth month as a Debian LTS and nineteenth month as a Debian ELTS paid contributor.  
I worked for 57.75 out of 59.50 hours for LTS and 42.25 out of 60.00 hours for ELTS.

#### LTS CVE Fixes and Announcements:

- Issued [DLA 2943-1](https://lists.debian.org/debian-lts-announce/2022/03/msg00015.html), fixing [CVE-2021-30151](https://security-tracker.debian.org/tracker/CVE-2021-30151) and [CVE-2022-23837](https://security-tracker.debian.org/tracker/CVE-2022-23837), for [ruby-sidekiq](https://tracker.debian.org/pkg/ruby-sidekiq).  
  For Debian 9 stretch, these problems have been fixed in version 4.2.3+dfsg-1+deb9u1.
- Issued [DLA 2951-1](https://lists.debian.org/debian-lts-announce/2022/03/msg00022.html), fixing [CVE-2021-0561](https://security-tracker.debian.org/tracker/CVE-2021-0561), for [flac](https://tracker.debian.org/pkg/flac).  
  For Debian 9 stretch, these problems have been fixed in version 1.3.2-2+deb9u2.
- Issued [DLA 2956-1](https://lists.debian.org/debian-lts-announce/2022/03/msg00028.html), fixing some vulnerabilties which haven't a CVE ID assigned yet, for [wordpress](https://tracker.debian.org/pkg/wordpress).  
  For Debian 9 stretch, these problems have been fixed in version 4.7.23+dfsg-0+deb9u1.
- Issued [DLA 2958-1](https://lists.debian.org/debian-lts-announce/2022/03/msg00030.html), fixing [CVE-2021-3700](https://security-tracker.debian.org/tracker/CVE-2021-3700), for [usbredir](https://tracker.debian.org/pkg/usbredir).  
  For Debian 9 stretch, these problems have been fixed in version 0.7.1-1+deb9u1.
- Issued [DLA 2936-1](https://lists.debian.org/debian-lts-announce/2022/03/msg00031.html), fixing [CVE-2018-8098](https://security-tracker.debian.org/tracker/CVE-2018-8098), [CVE-2018-8099](https://security-tracker.debian.org/tracker/CVE-2018-8099), [CVE-2018-10887](https://security-tracker.debian.org/tracker/CVE-2018-10887), [CVE-2018-10888](https://security-tracker.debian.org/tracker/CVE-2018-10888), [CVE-2018-15501](https://security-tracker.debian.org/tracker/CVE-2018-15501), [CVE-2020-12278](https://security-tracker.debian.org/tracker/CVE-2020-12278), [CVE-2020-12279](https://security-tracker.debian.org/tracker/CVE-2020-12279), [CVE-2019-1352](https://security-tracker.debian.org/tracker/CVE-2019-1352), and [CVE-2019-1353](https://security-tracker.debian.org/tracker/CVE-2019-1353), for [libgit2](https://tracker.debian.org/pkg/libgit2).  
  For Debian 9 stretch, these problems have been fixed in version 0.25.1+really0.24.6-1+deb9u1.
- Working on src:tiff and src:mbedtls to fix the issues, waiting for more issues to be reported, though.
- Help and assisted others w/ their queries, see "Other (E)LTS Work" section for more details.

#### ELTS CVE Fixes and Announcements:

- Issued [ELA 578-1](https://deb.freexian.com/extended-lts/updates/ela-578-1-flac/), fixing [CVE-2021-0561](https://security-tracker.debian.org/tracker/CVE-2021-0561), for [flac](https://tracker.debian.org/pkg/flac).  
  For Debian 8 jessie, these problems have been fixed in version 1.3.0-3+deb8u2.
- Issued [ELA 582-1](https://deb.freexian.com/extended-lts/updates/ela-582-1-wordpress/), fixing some vulnerabilties which haven't a CVE ID assigned yet, for [wordpress](https://tracker.debian.org/pkg/wordpress).  
  For Debian 8 jessie, these problems have been fixed in version 4.1.35+dfsg-0+deb8u1.
- Worked on readying up python2.7 update. But the tests fails with a segfault but only on jessie. The very same works fine on stretch.  
  Been trying to workthru the tests but it looks that it's a test-only thing. But I'll double-check to be sure. :)
- Looked into src:bind9 for Markus. Also, coordinated the same w/ the Ubuntu security team (ESM one). Reported the findings that I and Marc discussed.  
  Markus seemed to workthru a way out in the end. \o/
- Working on src:tiff and src:beep to fix the issues, waiting for more issues to be reported for src:tiff and src:beep is a bit of a PITA, though. :)

#### Other (E)LTS Work:

- Triaged [xterm](https://tracker.debian.org/pkg/xterm),
[dojo](https://tracker.debian.org/pkg/dojo),
[strongswan](https://tracker.debian.org/pkg/strongswan),
[ruby-sidekiq](https://tracker.debian.org/pkg/ruby-sidekiq),
[flac](https://tracker.debian.org/pkg/flac),
[wordpress](https://tracker.debian.org/pkg/wordpress),
[usbredir](https://tracker.debian.org/pkg/usbredir),
[debian-edu-config](https://tracker.debian.org/pkg/debian-edu-config),
[libphp-adodb](https://tracker.debian.org/pkg/libphp-adodb), and
[libgit2](https://tracker.debian.org/pkg/libgit2),
- Contributed to "Freexian values" (cf: internal survey).
- Read through the logs of the monthly Debian LTS meeting.
- Helped w/ debian-archive-keyring thread and gave pointers to Anton.
- Sorted out the [LXD VM issue for src:libgit2 upload](https://lists.debian.org/debian-lts/2022/03/msg00026.html).
- Helped answer Markus' question on src:bind9 security/regression updates.
- Answered questions (& discussions) on IRC (#debian-lts and #debian-elts).
- General and other discussions on LTS private and [public mailing list](https://lists.debian.org/debian-lts/2022/03/threads.html).
- Attended the monthly LTS meeting. Happened on #debian-lts this month.

#### Debian LTS Survey

I've spent 9 hours on the LTS survey on the following bits:  
(but I'll invoice them next month)
- Organize questions. Re-order, fix, and add things wherever needed.
- Finally set the whole thing up.
- Did a couple of dry-runs.
- Drafted the mail to be sent.

---

Until next time.  
`:wq` for today.
