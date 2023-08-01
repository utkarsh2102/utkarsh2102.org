+++
date = "2021-11-30 11:11:11 +0530"
title = "FOSS Activites in November 2021"
slug = "foss-in-nov-21"
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

Here's my (twenty-sixth) monthly but brief update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 35th month of actively contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March 2019 and a [DD](https://wiki.debian.org/DebianDeveloper) on Christmas '19! \o/

Just churning through the backlog again this month. Ugh.

Anyway, I did the following stuff in Debian:

#### Uploads and bug fixes:

- [rails](https://tracker.debian.org/pkg/rails) (2:6.1.4.1+dfsg-3) - No-change rebuild for unstable.

#### Other $things:

- Mentoring for newcomers.
- Moderation of -project mailing list.

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

This was my 10th month of actively contributing to [Ubuntu](https://ubuntu.com/about).
Now that I've joined [Canonical to work on Ubuntu full-time](https://utkarsh2102.org/posts/hello-canonical/), there's a bunch of things I do! \o/

I mostly worked on different things, I guess.

I was too lazy to maintain a list of things I worked on so there's
no concrete list atm. Maybe I'll get back to this section later or
will start to list stuff from next year onward, as I was doing before. :D

---

## Debian (E)LTS
{{< figure src="/images/debian-lts-small.png" >}}

[Debian Long Term Support (LTS)](https://www.freexian.com/en/services/debian-lts.html) is a project to extend the lifetime of all Debian stable releases to (at least) 5 years. Debian LTS is not handled by the Debian security team, but by a separate group of volunteers and companies interested in making it a success.  

And [Debian Extended LTS (ELTS)](https://deb.freexian.com/extended-lts) is its sister project, extending support to the Jessie release (+2 years after LTS support).

This was my twenty-sixth month as a Debian LTS and seventeenth month as a Debian ELTS paid contributor.  
I was assigned 30.00 hours for LTS and 45.00 hours for ELTS and worked on the following things:  

#### LTS CVE Fixes and Announcements:

- Issued [DLA 2813-1](), fixing [CVE-2021-33829](https://security-tracker.debian.org/tracker/CVE-2021-33829) and [CVE-2021-37695](https://security-tracker.debian.org/tracker/CVE-2021-37695), for [ckeditor](https://tracker.debian.org/pkg/ckeditor).  
  For Debian 9 stretch, these problems have been fixed in version 4.5.7+dfsg-2+deb9u1.
- Issued [DLA 2817-1](), fixing [CVE-2021-23214](https://security-tracker.debian.org/tracker/CVE-2021-23214) and [CVE-2021-23222](https://security-tracker.debian.org/tracker/CVE-2021-23222), for [postgresql-9.6](https://tracker.debian.org/pkg/postgresql-9.6).  
  For Debian 9 stretch, these problems have been fixed in version 9.6.24-0+deb9u1.
- Issued [DLA 2836-1](), fixing [CVE-2021-43527](https://security-tracker.debian.org/tracker/CVE-2021-43527), for [nss](https://tracker.debian.org/pkg/nss).  
  For Debian 9 stretch, these problems have been fixed in version 2:3.26.2-1.1+deb9u3.
- Started working on src:samba for CVE-2020-25717 to CVE-2020-25722 and CVE-2021-23192 for jessie and stretch, both.  
  The version difference b/w the suites are a bit too much for the patch(es) to be easily backported. I've talked to Anton to work something out. \o/
- Found the problem w/ libjdom1-java. Will have to roll the regression upload.  
  I've prepared the patch but needs some testing to be finally rolled out. Same for jessie.
- Started working on libgit2.

#### ELTS CVE Fixes and Announcements:

- Issued [ELA 523-1](), fixing [CVE-2021-33285](https://security-tracker.debian.org/tracker/CVE-2021-33285), [CVE-2021-33286](https://security-tracker.debian.org/tracker/CVE-2021-33286), [CVE-2021-33287](https://security-tracker.debian.org/tracker/CVE-2021-33287), [CVE-2021-33289](https://security-tracker.debian.org/tracker/CVE-2021-33289), [CVE-2021-35266](https://security-tracker.debian.org/tracker/CVE-2021-35266), [CVE-2021-35267](https://security-tracker.debian.org/tracker/CVE-2021-35267), [CVE-2021-35268](https://security-tracker.debian.org/tracker/CVE-2021-35268), [CVE-2021-35269](https://security-tracker.debian.org/tracker/CVE-2021-35269), [CVE-2021-39251](https://security-tracker.debian.org/tracker/CVE-2021-39251), [CVE-2021-39252](https://security-tracker.debian.org/tracker/CVE-2021-39252), [CVE-2021-39253](https://security-tracker.debian.org/tracker/CVE-2021-39253), [CVE-2021-39254](https://security-tracker.debian.org/tracker/CVE-2021-39254), [CVE-2021-39255](https://security-tracker.debian.org/tracker/CVE-2021-39255), [CVE-2021-39256](https://security-tracker.debian.org/tracker/CVE-2021-39256), [CVE-2021-39257](https://security-tracker.debian.org/tracker/CVE-2021-39257), [CVE-2021-39258](https://security-tracker.debian.org/tracker/CVE-2021-39258), [CVE-2021-39259](https://security-tracker.debian.org/tracker/CVE-2021-39259), [CVE-2021-39260](https://security-tracker.debian.org/tracker/CVE-2021-39260), [CVE-2021-39261](https://security-tracker.debian.org/tracker/CVE-2021-39261), [CVE-2021-39262](https://security-tracker.debian.org/tracker/CVE-2021-39262), and [CVE-2021-39263](https://security-tracker.debian.org/tracker/CVE-2021-39263), for [ntfs-3g](https://tracker.debian.org/pkg/ntfs-3g).  
  For Debian 8 jessie, these problems have been fixed in version 1:2014.2.15AR.2-1+deb8u5.
- Issued [ELA 524-1](), fixing [CVE-2021-43618](https://security-tracker.debian.org/tracker/CVE-2021-43618), for [gmp](https://tracker.debian.org/pkg/gmp).  
  For Debian 8 jessie, these problems have been fixed in version 2:6.0.0+dfsg-6+deb8u1.
- Issued [ELA 525-1](), fixing [CVE-2021-43527](https://security-tracker.debian.org/tracker/CVE-2021-43527), for [nss](https://tracker.debian.org/pkg/nss).  
  For Debian 8 jessie, these problems have been fixed in version 2:3.26-1+debu8u14.
- Started working on src:samba for CVE-2020-25717 to CVE-2020-25722 and CVE-2021-23192 for jessie and stretch, both.  
  The version difference b/w the suites are a bit too much for the patch(es) to be easily backported. I've talked to Anton to work something out. \o/
- Found the problem w/ libjdom1-java. Will have to roll the regression upload.  
  I've prepared the patch but needs some testing to be finally rolled out. Same for stretch.

#### Other (E)LTS Work:

- Front-desk duty from 29-11 to 05-12 for both LTS and ELTS.
- Triaged [udisk2](https://tracker.debian.org/pkg/udisks2),
[wordpress](https://tracker.debian.org/pkg/wordpress),
[samba](https://tracker.debian.org/pkg/samba),
[gmp](https://tracker.debian.org/pkg/gmp),
[nss](https://tracker.debian.org/pkg/nss),
[ntfs-3g](https://tracker.debian.org/pkg/ntfs-3g), and
[openssh](https://tracker.debian.org/pkg/openssh).
- Auto EOL'ed dwarfutils, radare2, mongodb, linux for jessie.
- As FD, did a deep dive into the no-pu-update issue. Will write to list shortly.
- Attended monthly Debian LTS meeting.
- Answered questions (& discussions) on IRC (#debian-lts and #debian-elts).
- General and other discussions on LTS private and [public mailing list](https://lists.debian.org/debian-lts/2021/11/threads.html).

#### Debian LTS Survey

I've spent 3 hours on the LTS survey on the following bits:
- Talking to Laura to revive the old a/c on survey.d.net.
- Setting up stuff there.
- Discussing the survey questions and other bits w/ Jeremiah.
- Partly reviewing the questions of the survey.
- Doing a walkthru of the LimeSurvey instance we have to make sure there are no "changes".

---

Until next time.  
`:wq` for today.
