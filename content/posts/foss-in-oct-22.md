+++
date = "2022-10-30 11:11:11 +0530"
title = "FOSS Activites in October 2022"
slug = "foss-in-oct-22"
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

Here's my (thirty-seventh) monthly but brief update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 46th month of actively contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March 2019 and a [DD](https://wiki.debian.org/DebianDeveloper) on Christmas '19! \o/

There's a bunch of things I do, both, technical and non-technical. Here are the things I did this month:

#### Debian Uploads

- [ruby-espeak](https://tracker.debian.org/pkg/ruby-espeak) (1.1.0-1) - New upstream version, v1.1.0.

#### Other $things:

- Being an AM for [Arun Kumar, process #1024](https://nm.debian.org/process/1024/). Process completed. \o/
- Sponsoring stuff for non-DDs.
- Mentoring for newcomers.
- Moderation of -project mailing list.

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

This was my 21st month of actively contributing to [Ubuntu](https://ubuntu.com/about).
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

This was my thirty-seventh month as a Debian LTS and twenty-eighth month as a Debian ELTS paid contributor.  
I worked for 35.00 hours for LTS and 25.00 hours for ELTS.

#### LTS CVE Fixes and Announcements:

- Issued [DLA 3146-1](https://lists.debian.org/debian-lts-announce/2022/10/msg00015.html), fixing [CVE-2022-2928](https://security-tracker.debian.org/tracker/CVE-2022-2928) and [CVE-2022-2929](https://security-tracker.debian.org/tracker/CVE-2022-2929), for [isc-dhcp](https://tracker.debian.org/pkg/isc-dhcp).  
  For Debian 10 buster, these problems have been fixed in version 4.4.1-2+deb10u2.
- Issued [DLA 3165-1](https://lists.debian.org/debian-lts-announce/2022/10/msg00033.html), fixing [CVE-2022-43680](https://security-tracker.debian.org/tracker/CVE-2022-43680), for [expat](https://tracker.debian.org/pkg/expat).  
  For Debian 10 buster, these problems have been fixed in version 2.2.6-2+deb10u6.
- Issued [DLA 3166-1](), fixing [CVE-2022-29970](https://security-tracker.debian.org/tracker/CVE-2022-29970), for [ruby-sinatra](https://tracker.debian.org/pkg/ruby-sinatra).  
  For Debian 10 buster, these problems have been fixed in version 2.0.5-4+deb10u1.
- Uploaded dropbear to fix CVE-2021-36369 in buster. Waiting for ELTS upload to issue the DLA. But will do soon now.
- src:joblib is a bit painful - having to backport patches to Py2. :/
- Started to look at other set of packages.

#### ELTS CVE Fixes and Announcements:

- Issued [ELA 715-1](https://www.freexian.com/lts/extended/updates/ela-715-1-expat/), fixing [CVE-2022-43680](https://security-tracker.debian.org/tracker/CVE-2022-43680), for [expat](https://tracker.debian.org/pkg/expat).  
  For Debian 9 stretch, these problems have been fixed in version 2.2.0-2+deb9u7.  
  For Debian 8 jessie, these problems have been fixed in version 2.1.0-6+deb8u10.
- Issued [ELA 716-1](https://www.freexian.com/lts/extended/updates/ela-716-1-djangorestframework/), fixing [CVE-2018-25045](https://security-tracker.debian.org/tracker/CVE-2018-25045) and [CVE-2020-25626](https://security-tracker.debian.org/tracker/CVE-2020-25626), for [djangorestframework](https://tracker.debian.org/pkg/djangorestframework).  
  For Debian 9 stretch, these problems have been fixed in version 3.4.0-2+deb9u1.
- Uploaded dropbear to fix CVE-2021-36369 in buster. Waiting for ELTS upload, too. But some backporting problems. :/
- src:joblib is a bit painful - having to backport patches to Py2. :/
- Started to look at other set of packages.

#### Other (E)LTS Work:

- Triaged [joblib](https://tracker.debian.org/pkg/joblib),
[dropbear](https://tracker.debian.org/pkg/dropbear),
[ruby-sinatra](https://tracker.debian.org/pkg/ruby-sinatra),
[djangorestframework](https://tracker.debian.org/pkg/djangorestframework),
[isc-dhcp](https://tracker.debian.org/pkg/isc-dhcp), and
[expat](https://tracker.debian.org/pkg/expat).
- Reverted "Mark freerdp CVEs wrongly affecting freerdp <2.0.0" in the ELTS tracker.
- Helped and assisted new contributors joining Freexian (LTS/ELTS).
- Answered questions (& discussions) on IRC (#debian-lts and #debian-elts) and Matrix.
- Participated and helped fellow members with their queries via private mail and chat.
- General and other discussions on LTS private and [public mailing list](https://lists.debian.org/debian-lts/2022/10/threads.html).
- Attended the monthly meeting held on Jitsi on October 27th.

---

Until next time.  
`:wq` for today.
