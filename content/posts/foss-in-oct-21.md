+++
date = "2021-11-01 11:11:11 +0530"
title = "FOSS Activites in October 2021"
slug = "foss-in-oct-21"
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

Here's my (twenty-fifth) monthly but brief update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 34th month of actively contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March 2019 and a [DD](https://wiki.debian.org/DebianDeveloper) on Christmas '19! \o/

Just churning through the backlog again this month. Ugh.

Anyway, I did the following stuff in Debian:

#### Uploads and bug fixes:

Hah, as a surprise, I did no uploads or bug fixes this month. :(

#### Other $things:

- Mentoring for newcomers.
- Moderation of -project mailing list.

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

This was my 9th month of actively contributing to [Ubuntu](https://ubuntu.com/about).
Now that I've joined [Canonical to work on Ubuntu full-time](https://utkarsh2102.com/posts/hello-canonical/), there's a bunch of things I do! \o/

I mostly worked on different things, I guess.

I was too lazy to maintain a list of things I worked on so there's
no concrete list atm. Maybe I'll get back to this section later or
will start to list stuff from next year onward, as I was doing before. :D

---

## Debian (E)LTS
{{< figure src="/images/debian-lts-small.png" >}}

[Debian Long Term Support (LTS)](https://www.freexian.com/en/services/debian-lts.html) is a project to extend the lifetime of all Debian stable releases to (at least) 5 years. Debian LTS is not handled by the Debian security team, but by a separate group of volunteers and companies interested in making it a success.  

And [Debian Extended LTS (ELTS)](https://deb.freexian.com/extended-lts) is its sister project, extending support to the Jessie release (+2 years after LTS support).

This was my twenty-fifth month as a Debian LTS and sixteenth month as a Debian ELTS paid contributor.  
I was assigned 28.50 hours for LTS and 40.00 hours for ELTS and worked on the following things:  
(however, I only worked for 35h on ELTS work, thereby, carrying over a few hours.)

#### LTS CVE Fixes and Announcements:

- Issued [DLA 2780-1](), fixing [CVE-2021-31799](https://security-tracker.debian.org/tracker/CVE-2021-31799), [CVE-2021-31810](https://security-tracker.debian.org/tracker/CVE-2021-31810), and [CVE-2021-32066](https://security-tracker.debian.org/tracker/CVE-2021-32066), for [ruby2.3](https://tracker.debian.org/pkg/ruby2.3).  
  For Debian 9 stretch, these problems have been fixed in version 2.3.3-1+deb9u10.
- Issued [DLA 2743-2](), fixing [CVE-2017-5715](https://security-tracker.debian.org/tracker/CVE-2017-5715), for [amd64-microcode](https://tracker.debian.org/pkg/amd64-microcode).  
  For Debian 9 stretch, these problems have been fixed in version 3.20181128.1~deb9u2.  
  This update took the most time as this had to be co-ordinated w/ multiple people and teams. But finally got this sorted! \o/
- Issued [DLA 2808-1](), fixing [CVE-2021-3733](https://security-tracker.debian.org/tracker/CVE-2021-3733) and [CVE-2021-3737](https://security-tracker.debian.org/tracker/CVE-2021-3737), for [python3.5](https://tracker.debian.org/pkg/python3.5).  
  For Debian 9 stretch, these problems have been fixed in version 3.5.3-1+deb9u5.
- Prepped the debian-archive-keyring update, however the build fails because of Jonathan's GPG keys.
  Wrote to the list and Jonathan replied that they'll prep a branch that I can land later. So waiting on that.

#### ELTS CVE Fixes and Announcements:

- Issued [ELA 510-1](), fixing [CVE-2021-3426](https://security-tracker.debian.org/tracker/CVE-2021-3426), [CVE-2021-3733](https://security-tracker.debian.org/tracker/CVE-2021-3733), and [CVE-2021-3737](https://security-tracker.debian.org/tracker/CVE-2021-3737), for [python3.4](https://tracker.debian.org/pkg/python3.4).  
  For Debian 8 jessie, these problems have been fixed in version 3.4.2-1+deb8u11.
- Issued [ELA 513-1](), fixing [CVE-2021-33829](https://security-tracker.debian.org/tracker/CVE-2021-33829) and [CVE-2021-37695](https://security-tracker.debian.org/tracker/CVE-2021-37695), for [ckeditor](https://tracker.debian.org/pkg/ckeditor).  
  For Debian 8 jessie, these problems have been fixed in version 4.4.4+dfsg1-3+deb8u1.
- Took a look at jsoup again. Post-discussion, the customer did not revert, so we decided to ignore the CVEs.
- Worked on openssh's reported regression ([via LP: #1934501](https://bugs.launchpad.net/ubuntu/+source/openssh/+bug/1934501)) and found that Debian
  jessie, stretch, buster, and bullseye aren't affected. Informed the security team as well (whom I woked along with). Given that all seemed in order,
  we decided to postpone the new CVE since that was a minor issue which can be piggy-backed later with a more severe issue.
- Co-ordinated with Abhijith who unclaimed ntfs-3g and started working on the update. A high number of CVEs are open. Work still in progress.

#### Other (E)LTS Work:

- Front-desk duty from 30-08 until 05-09 and 27-09 to 03-10 for both LTS and ELTS.
- Triaged [ffmpeg](https://tracker.debian.org/pkg/ffmpeg),
[git](https://tracker.debian.org/pkg/git),
[gpac](https://tracker.debian.org/pkg/gpac),
[inetutils](https://tracker.debian.org/pkg/inetutils),
[mc](https://tracker.debian.org/pkg/mc),
[modsecurity-crs](https://tracker.debian.org/pkg/modsecurity-crs),
[node-object-path](https://tracker.debian.org/pkg/node-object-path),
[php-pear](https://tracker.debian.org/pkg/php-pear),
[systemd-cron](https://tracker.debian.org/pkg/systemd-cron),
[node-tar](https://tracker.debian.org/pkg/node-tar),
[ruby2.3](https://tracker.debian.org/pkg/ruby2.3),
[gst-plugins-bad0.10](https://tracker.debian.org/pkg/gst-plugins-bad0.10),
[ntfs-3g](https://tracker.debian.org/pkg/ntfs-3g),
[tiff](https://tracker.debian.org/pkg/tiff),
[wordpress](https://tracker.debian.org/pkg/wordpress), and
[openssh](https://tracker.debian.org/pkg/openssh).
- Mark CVE-2021-38171/ffmpeg as postponed for stretch.
- Mark CVE-2021-40330/git as no-dsa for stretch and jessie.
- Mark CVE-2020-19481/gpac as ignored for stretch.
- Mark CVE-2021-40491/inetutils as no-dsa for stretch.
- Mark CVE-2021-36370/mc as no-dsa for stretch and jessie.
- Mark CVE-2021-35368/modsecurity-crs as no-dsa for stretch.
- Mark CVE-2021-23434/node-object-path as end-of-life for stretch.
- Mark CVE-2021-32610/php-pear as no-dsa for stretch.
- Mark CVE-2017-9525/systemd-cron as no-dsa for stretch.
- Mark CVE-2021-37701/node-tar as end-of-life for stretch.
- Mark CVE-2021-37712/node-tar as end-of-life in stretch.
- Mark CVE-2021-39201/wordpress as not-affected for jessie.
- Mark CVE-2020-19143/tiff as not-affected for stretch and jessie.
- Auto EOL'ed gpac, nltk, request-tracker4, and linux for jessie.
- Drop wordpress from {d,e}la-needed for stretch and jessie. No update needed.
- Drop qtbase-opensource-src from dla-needed for stretch. CVE-2020-24742 has the same fix as CVE-2020-0569.
- A backporting error for CVE-2018-15473 was reported in Ubuntu (and can see the same code differences here). This needs further deeper investigation w/ Ubuntu and Debian security teams involved.
- Attended monthly Debian LTS meeting.
- Answered questions (& discussions) on IRC (#debian-lts and #debian-elts).
- General and other discussions on LTS private and [public mailing list](https://lists.debian.org/debian-lts/2021/09/threads.html).

---

Until next time.  
`:wq` for today.
