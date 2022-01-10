+++
date = "2022-01-01 11:11:11 +0530"
title = "FOSS Activites in December 2021"
slug = "foss-in-dec-21"
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

Here's my (twenty-seventh) monthly but brief update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 36th month of actively contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March 2019 and a [DD](https://wiki.debian.org/DebianDeveloper) on Christmas '19! \o/

Just churning through the backlog again this month. Ugh.

Anyway, I did the following stuff in Debian:

#### Uploads and bug fixes:

- [ruby2.7](https://tracker.debian.org/pkg/ruby2.7) (2.7.5-1) - New upstream version fixing 3 new CVEs.

#### Other $things:

- Mentoring for newcomers.
- Moderation of -project mailing list.

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

This was my 11th month of actively contributing to [Ubuntu](https://ubuntu.com/about).
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

This was my twenty-seventh month as a Debian LTS and eighteenth month as a Debian ELTS paid contributor.  
I was assigned 40.00 hours for LTS and 60.00 hours for ELTS and worked on the following things:  
(since I had a 3-week vacation, I wanted to wrap things up that were pending and so I worked for 20h more for LTS, which I'll compensate the next month!)


#### LTS CVE Fixes and Announcements:

- Issued [DLA 2844-1](), fixing [CVE-2021-44540](https://security-tracker.debian.org/tracker/CVE-2021-44540) and [CVE-2021-44543](https://security-tracker.debian.org/tracker/CVE-2021-44543), for [privoxy](https://tracker.debian.org/pkg/privoxy).  
  For Debian 9 stretch, these problems have been fixed in version 3.0.26-3+deb9u3.
- Issued [DLA 2847-1](), fixing [CVE-2021-44858](https://security-tracker.debian.org/tracker/CVE-2021-44858), for [mediawiki](https://tracker.debian.org/pkg/mediawiki).  
  For Debian 9 stretch, these problems have been fixed in version 1:1.27.7-1+deb9u11.
- Issued [DLA 2853-1](), fixing [CVE-2021-41817](https://security-tracker.debian.org/tracker/CVE-2021-41817) and [CVE-2021-41819](https://security-tracker.debian.org/tracker/CVE-2021-41819), for [ruby2.3](https://tracker.debian.org/pkg/ruby2.3).  
  For Debian 9 stretch, these problems have been fixed in version 2.3.3-1+deb9u11.
- Issued [DLA 2854-1](), fixing [CVE-2017-18635](https://security-tracker.debian.org/tracker/CVE-2017-18635), for [novnc](https://tracker.debian.org/pkg/novnc).  
  For Debian 9 stretch, these problems have been fixed in version 1:0.4+dfsg+1+20131010+gitf68af8af3d-6+deb9u1.
- Issued [DLA 2860-1](), fixing [CVE-2018-7750](https://security-tracker.debian.org/tracker/CVE-2018-7750) and [CVE-2018-1000805](https://security-tracker.debian.org/tracker/CVE-2018-1000805), for [paramiko](https://tracker.debian.org/pkg/paramiko).  
  For Debian 9 stretch, these problems have been fixed in version 2.0.0-1+deb9u1.
- Issued [DLA 2862-1](), fixing [CVE-2018-12020](https://security-tracker.debian.org/tracker/CVE-2018-12020) and [CVE-2019-6690](https://security-tracker.debian.org/tracker/CVE-2019-6690), for [python-gnupg](https://tracker.debian.org/pkg/python-gnupg).  
  For Debian 9 stretch, these problems have been fixed in version 0.3.9-1+deb9u1.
- Issued [DLA 2864-1](), fixing [CVE-2017-1002201](https://security-tracker.debian.org/tracker/CVE-2017-1002201), for [ruby-haml](https://tracker.debian.org/pkg/ruby-haml).  
  For Debian 9 stretch, these problems have been fixed in version 4.0.7-1+deb9u1.
- Issued [DLA 2871-1](), fixing [CVE-2021-43818](https://security-tracker.debian.org/tracker/CVE-2021-43818), for [lxml](https://tracker.debian.org/pkg/lxml).  
  For Debian 9 stretch, these problems have been fixed in version 3.7.1-1+deb9u5.
- Simultaneously, I've been working on rolling the samba update. Should happen the next month.

#### ELTS CVE Fixes and Announcements:

- Issued [ELA 525-2](), fixing [CVE-2021-43527](https://security-tracker.debian.org/tracker/CVE-2021-43527), for [nss](https://tracker.debian.org/pkg/nss).  
  For Debian 8 jessie, these problems have been fixed in version 2:3.26-1+debu8u15.
- Issued [ELA 530-1](), for [systemd](https://tracker.debian.org/pkg/systemd).  
  For Debian 8 jessie, these problems have been fixed in version 215-17+deb8u14.
- Issued [ELA 531-1](), fixing [CVE-2021-41817](https://security-tracker.debian.org/tracker/CVE-2021-41817) and [CVE-2021-41819](https://security-tracker.debian.org/tracker/CVE-2021-41819), for [ruby2.1](https://tracker.debian.org/pkg/ruby2.1).  
  For Debian 8 jessie, these problems have been fixed in version 2.1.5-2+deb8u13.
- Issued [ELA 533-1](), fixing [CVE-2018-12020](https://security-tracker.debian.org/tracker/CVE-2018-12020), for [python-gnupg](https://tracker.debian.org/pkg/python-gnupg).  
  For Debian 8 jessie, these problems have been fixed in version 0.3.6-1+deb8u2.
- Issued [ELA 536-1](), fixing [CVE-2021-43818](https://security-tracker.debian.org/tracker/CVE-2021-43818), for [lxml](https://tracker.debian.org/pkg/lxml).  
  For Debian 8 jessie, these problems have been fixed in version Prior to version 4.6.5, the HTML Cleaner in lxml.html lets certain.
- Started working on src:samba for CVE-2020-25717 to CVE-2020-25722 and CVE-2021-23192 for jessie and stretch, both.  
  The version difference b/w the suites are a bit too much for the patch(es) to be easily backported. I've talked to Anton to work something out. \o/
- Found the problem w/ libjdom1-java. Will have to roll the regression upload.  
  I've prepared the patch but needs some testing to be finally rolled out. Same for stretch.

#### Other (E)LTS Work:

- Front-desk duty from 29-11 to 05-12 and 20-12 to 26-12 for both LTS and ELTS.
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
[npm](https://tracker.debian.org/pkg/npm),
[nltk](https://tracker.debian.org/pkg/nltk),
[request-tracker4](https://tracker.debian.org/pkg/request-tracker4),
[ros-ros-comm](https://tracker.debian.org/pkg/ros-ros-comm),
[mediawiki](https://tracker.debian.org/pkg/mediawiki),
[ruby2.1](https://tracker.debian.org/pkg/ruby2.1),
[ckeditor](https://tracker.debian.org/pkg/ckeditor),
[ntfs-3g](https://tracker.debian.org/pkg/ntfs-3g),
[tiff](https://tracker.debian.org/pkg/tiff),
[wordpress](https://tracker.debian.org/pkg/wordpress), and
[jsoup](https://tracker.debian.org/pkg/jsoup),
[udisks2](https://tracker.debian.org/pkg/udisks2),
[libgit2](https://tracker.debian.org/pkg/libgit2),
[python3.5](https://tracker.debian.org/pkg/python3.5),
[python3.4](https://tracker.debian.org/pkg/python3.4), and
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
- Mark CVE-2021-38562/request-tracker4 as no-dsa for stretch.
- Mark CVE-2021-37146/ros-ros-comm as no-dsa for stretch.
- Mark CVE-2021-28965/ruby2.1 as ignored for jessie.
- Mark CVE-2021-37714/jsoup as ignored for jessie.
- Mark CVE-2021-41617/openssh as no-dsa for jessie.
- Auto EOL'ed ardour, nltk, request-tracker4, python-scrapy, webkit2gtk, and linux for jessie.
- Attended monthly Debian LTS meeting.
- Answered questions (& discussions) on IRC (#debian-lts and #debian-elts).
- General and other discussions on LTS private and [public mailing list](https://lists.debian.org/debian-lts/2021/12/threads.html).

#### Debian LTS Survey

I've spent 5 hours on the LTS survey on the following bits:
- Went through the old content on the previous survey.
- Reviewed the new content - still more work to do.
- Discussed the survey bits in the team meeting.
- Partly reviewing the questions of the survey.
- Walking through the instance to find the doability of the tasks discussed in the meeting.
- Segregating and staging questions. More work to do here.

---

Until next time.  
`:wq` for today.
