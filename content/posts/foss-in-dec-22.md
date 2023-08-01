+++
date = "2022-12-30 11:11:11 +0530"
title = "FOSS Activites in December 2022"
slug = "foss-in-dec-22"
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

Here's my (thirty-ninth) monthly but brief update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 48th month of actively contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March 2019 and a [DD](https://wiki.debian.org/DebianDeveloper) on Christmas '19! \o/

There's a bunch of things I do, both, technical and non-technical. Here are the things I did this month:

- Some DebConf work.
- Sponsoring stuff for non-DDs.
- Mentoring for newcomers.
- Moderation of -project mailing list.

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

This was my 23rd month of actively contributing to [Ubuntu](https://ubuntu.com/about).
Now that I joined [Canonical to work on Ubuntu full-time](https://utkarsh2102.org/posts/hello-canonical/), there's a bunch of things I do! \o/

I mostly worked on different things, I guess.

I was too lazy to maintain a list of things I worked on so there's
no concrete list atm. Maybe I'll get back to this section later or
will start to list stuff from the fall, as I was doing before. :D

---

## Debian (E)LTS
{{< figure src="/images/debian-lts-small.png" >}}

[Debian Long Term Support (LTS)](https://www.freexian.com/en/services/debian-lts.html) is a project to extend the lifetime of all Debian stable releases to (at least) 5 years. Debian LTS is not handled by the Debian security team, but by a separate group of volunteers and companies interested in making it a success.  

And [Debian Extended LTS (ELTS)](https://deb.freexian.com/extended-lts) is its sister project, extending support to the stretch and jessie release (+2 years after LTS support).

This was my thirty-ninth month as a Debian LTS and thirtieth month as a Debian ELTS paid contributor.  
I worked for 51.50 hours for LTS and 22.50 hours for ELTS.

#### LTS CVE Fixes and Announcements:

- Issued [DLA 3224-1](https://lists.debian.org/debian-lts-announce/2022/12/msg00009.html), fixing [CVE-2020-8287](https://security-tracker.debian.org/tracker/CVE-2020-8287), for [http-parser](https://tracker.debian.org/pkg/http-parser).  
  For Debian 10 buster, these problems have been fixed in version 2.8.1-1+deb10u3.
- Issued [DLA 3225-1](https://lists.debian.org/debian-lts-announce/2022/12/msg00010.html), fixing [CVE-2022-46391](https://security-tracker.debian.org/tracker/CVE-2022-46391), for [awstats](https://tracker.debian.org/pkg/awstats).  
  For Debian 10 buster, these problems have been fixed in version 7.6+dfsg-2+deb10u2.
- Issued [DLA 3227-1](https://lists.debian.org/debian-lts-announce/2022/12/msg00012.html), fixing [CVE-2022-32209](https://security-tracker.debian.org/tracker/CVE-2022-32209), for [ruby-rails-html-sanitizer](https://tracker.debian.org/pkg/ruby-rails-html-sanitizer).  
  For Debian 10 buster, these problems have been fixed in version 1.0.4-1+deb10u1.
- Issued [DLA 3228-1](https://lists.debian.org/debian-lts-announce/2022/12/msg00013.html), fixing [CVE-2021-3918](https://security-tracker.debian.org/tracker/CVE-2021-3918), for [node-json-schema](https://tracker.debian.org/pkg/node-json-schema).  
  For Debian 10 buster, these problems have been fixed in version 0.2.3-1+deb10u1.
- Issued [DLA 3229-1](https://lists.debian.org/debian-lts-announce/2022/12/msg00014.html), fixing [CVE-2022-21704](https://security-tracker.debian.org/tracker/CVE-2022-21704), for [node-log4js](https://tracker.debian.org/pkg/node-log4js).  
  For Debian 10 buster, these problems have been fixed in version 4.0.2-2+deb10u1.
- Issued [DLA 3230-1](https://lists.debian.org/debian-lts-announce/2022/12/msg00015.html), fixing [CVE-2021-41182](https://security-tracker.debian.org/tracker/CVE-2021-41182), [CVE-2021-41183](https://security-tracker.debian.org/tracker/CVE-2021-41183), [CVE-2021-41184](https://security-tracker.debian.org/tracker/CVE-2021-41184), and [CVE-2022-31160](https://security-tracker.debian.org/tracker/CVE-2022-31160), for [jqueryui](https://tracker.debian.org/pkg/jqueryui).  
  For Debian 10 buster, these problems have been fixed in version 1.12.1+dfsg-5+deb10u1.
- Issued [DLA 3231-1](https://lists.debian.org/debian-lts-announce/2022/12/msg00016.html), fixing [CVE-2020-29394](https://security-tracker.debian.org/tracker/CVE-2020-29394), [CVE-2020-36244](https://security-tracker.debian.org/tracker/CVE-2020-36244), and [CVE-2022-31291](https://security-tracker.debian.org/tracker/CVE-2022-31291), for [dlt-daemon](https://tracker.debian.org/pkg/dlt-daemon).  
  For Debian 10 buster, these problems have been fixed in version 2.18.0-1+deb10u1.
- Inspected joblib's security update upon Helmut's investigation and see what went wrong there.
- Started to look at other set of packages: node-moment, tiff, ruby*, et al.

#### ELTS CVE Fixes and Announcements:

- Issued [ELA 752-1](https://www.freexian.com/lts/extended/updates/ela-752-1-jqueryui/), fixing [CVE-2021-41182](https://security-tracker.debian.org/tracker/CVE-2021-41182), [CVE-2021-41183](https://security-tracker.debian.org/tracker/CVE-2021-41183), [CVE-2021-41184](https://security-tracker.debian.org/tracker/CVE-2021-41184), and [CVE-2022-31160](https://security-tracker.debian.org/tracker/CVE-2022-31160), for [jqueryui](https://tracker.debian.org/pkg/jqueryui).  
  For Debian 9 stretch, these problems have been fixed in version 1.12.1+dfsg-4+deb9u1.
- Helped facilitate Erlang's and RabbitMQ's update; cf: [ELA 754-1](https://www.freexian.com/lts/extended/updates/ela-754-1-erlang/).
- Looked through python3.4's FTBFS on armhf. Even diff'd with Ubuntu. No luck. Inspected the traces, doesn't give a lot of hint either. Will continue to look later next month or so but it's a rabbit hole. (:
- Inspected joblib's security update upon Helmut's investigation and see what went wrong there.
- Started to look at other set of packages: dropbear, tiff, et al.

#### Other (E)LTS Work:

- Triaged [jqueryui](https://tracker.debian.org/pkg/jqueryui),
[http-parser](https://tracker.debian.org/pkg/http-parser),
[awstats](https://tracker.debian.org/pkg/awstats),
[ruby-rails-html-sanitizer](https://tracker.debian.org/pkg/ruby-rails-html-sanitizer),
[node-json-schema](https://tracker.debian.org/pkg/node-json-schema),
[node-log4js](https://tracker.debian.org/pkg/node-log4js),
[dlt-daemon](https://tracker.debian.org/pkg/dlt-daemon),
[joblib](https://tracker.debian.org/pkg/joblib),
[tiff](https://tracker.debian.org/pkg/tiff),
[dropbear](https://tracker.debian.org/pkg/dropbear),
[python3.5](https://tracker.debian.org/pkg/python3.5),
[python3.4](https://tracker.debian.org/pkg/python3.4),
[ruby-sinatra](https://tracker.debian.org/pkg/ruby-sinatra),
[erlang](https://tracker.debian.org/pkg/erlang), and
[rabbitmq-server](https://tracker.debian.org/pkg/rabbitmq-server).
- Helped and assisted new contributors joining Freexian (LTS/ELTS/internally).
- Answered questions (& discussions) on IRC (#debian-lts and #debian-elts) and Matrix.
- Participated and helped fellow members with their queries via private mail and chat.
- General and other discussions on LTS private and [public mailing list](https://lists.debian.org/debian-lts/2022/12/threads.html).
- Attended the monthly Freexian meeting.

---

Until next time.  
`:wq` for today.
