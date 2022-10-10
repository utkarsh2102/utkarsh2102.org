+++
date = "2022-05-30 11:11:11 +0530"
title = "FOSS Activites in May 2022"
slug = "foss-in-may-22"
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

Here's my (thirty-second) monthly but brief update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 41st month of actively contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March 2019 and a [DD](https://wiki.debian.org/DebianDeveloper) on Christmas '19! \o/

There's a bunch of things I did this month but mostly non-technical, now that DC22 is around the corner. Here are the things I did:

#### Debian Uploads

- [puppet-beaker](https://tracker.debian.org/pkg/puppet-beaker) (4.30.0-2) - Sponsored the upload to fix net-ssh's FTBFS.
- [ruby-terminal-table](https://tracker.debian.org/pkg/ruby-terminal-table) (3.0.2-1) - New upstream version, v3.0.2.

#### Other $things:

- Volunteering for DC22 Content team.
- Leading the Bursary team w/ Paulo.
- Answering a bunch of questions and things bursary.
- Being an AM for [Arun Kumar, process #1024](https://nm.debian.org/process/1024/).
- Mentoring for newcomers.
- Moderation of -project mailing list.

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

This was my 16th month of actively contributing to [Ubuntu](https://ubuntu.com/about).
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

This was my thirty-second month as a Debian LTS and twenty-third month as a Debian ELTS paid contributor.  
I worked for 35.00 hours for LTS and 30.00 hours for ELTS.

#### LTS CVE Fixes and Announcements:

- Issued [DLA 2999-1](https://lists.debian.org/debian-lts-announce/2022/05/msg00010.html), fixing [CVE-2022-1328](https://security-tracker.debian.org/tracker/CVE-2022-1328), for [mutt](https://tracker.debian.org/pkg/mutt).  
  For Debian 9 stretch, these problems have been fixed in version 1.7.2-1+deb9u6.
- Issued [DLA 3009-1](https://lists.debian.org/debian-lts-announce/2022/05/msg00020.html), fixing [CVE-2022-27239](https://security-tracker.debian.org/tracker/CVE-2022-27239) and [CVE-2022-29869](https://security-tracker.debian.org/tracker/CVE-2022-29869), for [cifs-utils](https://tracker.debian.org/pkg/cifs-utils).  
  For Debian 9 stretch, these problems have been fixed in version 2:6.7-1+deb9u1.
- Issued [DLA 3013-1](https://lists.debian.org/debian-lts-announce/2022/05/msg00024.html), fixing [CVE-2022-30688](https://security-tracker.debian.org/tracker/CVE-2022-30688), for [needrestart](https://tracker.debian.org/pkg/needrestart).  
  For Debian 9 stretch, these problems have been fixed in version 2.11-3+deb9u2.
- Issued [DLA 3014-1](https://lists.debian.org/debian-lts-announce/2022/05/msg00025.html), fixing [CVE-2020-8659](https://security-tracker.debian.org/tracker/CVE-2020-8659), for [elog](https://tracker.debian.org/pkg/elog).  
  For Debian 9 stretch, these problems have been fixed in version 3.1.2-1-1+deb9u1.
- Issued [DLA 3038-1](https://lists.debian.org/debian-lts-announce/2022/06/msg00000.html), for [debian-security-support](https://tracker.debian.org/pkg/debian-security-support).  
  For Debian 9 stretch, these problems have been fixed in version 1:9+2022.06.02.
- Working on tiff update for stretch.

#### ELTS CVE Fixes and Announcements:

- Issued [ELA 607-1](), fixing [CVE-2022-1328](https://security-tracker.debian.org/tracker/CVE-2022-1328), for [mutt](https://tracker.debian.org/pkg/mutt).  
  For Debian 8 jessie, these problems have been fixed in version 1.5.23-3+deb8u6.
- Issued [ELA 608-1](), fixing [CVE-2022-28044](https://security-tracker.debian.org/tracker/CVE-2022-28044), for [lrzip](https://tracker.debian.org/pkg/lrzip).  
  For Debian 8 jessie, these problems have been fixed in version 0.616-1+deb8u2.
- Issued [ELA 611-1](), fixing [CVE-2022-25647](https://security-tracker.debian.org/tracker/CVE-2022-25647), for [libgoogle-gson-java](https://tracker.debian.org/pkg/libgoogle-gson-java).  
  For Debian 8 jessie, these problems have been fixed in version 2.2.4-1+deb8u1.
- Issued [ELA 614-1](), fixing [CVE-2022-27239](https://security-tracker.debian.org/tracker/CVE-2022-27239) and [CVE-2022-29869](https://security-tracker.debian.org/tracker/CVE-2022-29869), for [cifs-utils](https://tracker.debian.org/pkg/cifs-utils).  
  For Debian 8 jessie, these problems have been fixed in version 2:6.4-1+deb8u1.
- Working on tiff and beep updates for jessie.

#### Other (E)LTS Work:

- Triaged [cifs-utils](https://tracker.debian.org/pkg/cifs-utils),
[vim](https://tracker.debian.org/pkg/vim),
[elog](https://tracker.debian.org/pkg/elog),
[needrestart](https://tracker.debian.org/pkg/needrestart),
[amd64-microcode](https://tracker.debian.org/pkg/amd64-microcode),
[libgoogle-gson-java](https://tracker.debian.org/pkg/libgoogle-gson-java),
[lrzip](https://tracker.debian.org/pkg/lrzip), and
[mutt](https://tracker.debian.org/pkg/mutt).
- Started as a Freexian Collaborator! \o/
- Read through the documentation bits around that.
- Helped and assisted new contributors joining Freexian.
- Answered questions (& discussions) on IRC (#debian-lts and #debian-elts).
- Participated and helped fellow members with theie queries via private mail and chat.
- General and other discussions on LTS private and [public mailing list](https://lists.debian.org/debian-lts/2022/05/threads.html).

#### Debian LTS Survey

I've spent 2 hours on the LTS survey on the following bits:  
- Finalizing and wrapping up the survey.
- Providing the stats, working on the initial export of the survey.
- Dropping ghost entries and other things which are useless. :)

---

Until next time.  
`:wq` for today.
