+++
date = "2022-06-30 11:11:11 +0530"
title = "FOSS Activites in June 2022"
slug = "foss-in-june-22"
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

Here's my (thirty-third) monthly but brief update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 42nd month of actively contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March 2019 and a [DD](https://wiki.debian.org/DebianDeveloper) on Christmas '19! \o/

There's a bunch of things I did this month but mostly non-technical, now that DC22 is around the corner. Here are the things I did:

#### Debian Uploads

- [ruby-image-processing](https://tracker.debian.org/pkg/ruby-image-processing) (1.10.3-2) - Add patch to fix remote shell execution in #apply. (Closes: #1007225)

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

This was my 17th month of actively contributing to [Ubuntu](https://ubuntu.com/about).
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

This was my thirty-third month as a Debian LTS and twenty-fourth month as a Debian ELTS paid contributor.  
I worked for 6.50 hours for LTS and 4.75 hours for ELTS.

#### LTS CVE Fixes and Announcements:

- Issued DLA 3048-1, fixing CVE-2022-31799, for python-bottle.
- Started to work on CVE-2020-36475, CVE-2020-36476, CVE-2020-36478, CVE-2021-24119, CVE-2021-43666, and CVE-2021-44732	for mbedtls.
- Re-started working on the tiff update.

#### ELTS CVE Fixes and Announcements:

- Issued ELA 621-1, fixing CVE-2018-1000532, for beep.
- Issued ELA 623-1, fixing CVE-2022-31799, for python-bottle.
- Re-started working on the tiff update.

#### Other (E)LTS Work:

- Triaged [beep](https://tracker.debian.org/pkg/beep),
[python-bottle](https://tracker.debian.org/pkg/python-bottle),
[tiff](https://tracker.debian.org/pkg/tiff), and
[mbedtls](https://tracker.debian.org/pkg/mbedtls),
- Started as a Freexian Collaborator last month! \o/
- Moar reading on the documentation bits.
- Helped and assisted new contributors joining Freexian.
- Answered questions (& discussions) on IRC (#debian-lts and #debian-elts).
- Participated and helped fellow members with theie queries via private mail and chat.
- General and other discussions on LTS private and [public mailing list](https://lists.debian.org/debian-lts/2022/06/threads.html).

#### Debian LTS Survey

I've spent 9 hours on the LTS survey on the following bits:
- Importing the "useful" data and sorting it out and downloading the available graphs on the LS instance.
- Figured that the LS data is not very clear and in some cases, pretty useless. Sigh.
- Started writing the final document in LaTeX.
- Screenshotted the graphs (neatly) and arranged them in the LaTeX docuement.
- Readied it up to present in DebConf, during the LTS BoF. \o/

---

Until next time.  
`:wq` for today.
