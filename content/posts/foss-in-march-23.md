+++
date = "2023-03-30 11:11:11 +0530"
title = "FOSS Activites in March 2023"
slug = "foss-in-march-23"
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

Here's my (forty-second) monthly but brief update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 51st month of actively contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March 2019 and a [DD](https://wiki.debian.org/DebianDeveloper) on Christmas '19! \o/

There's a bunch of things I do, both, technical and non-technical. Here are the things I did this month:

### Uploads


### Others

- Looked up some Release team documentation.
- Mentoring for newcomers.
- Ruby sprints.
- Bug work (on BTS and #debian-ruby) for rails and redmine.
- Moderation of -project mailing list.

A huge thanks to Freexian for sponsoring my Debian work and Entrouvert for sponsoring the Redmine backports. :D

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

This was my 26th month of actively contributing to [Ubuntu](https://ubuntu.com/about).
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

This was my forty-second month as a Debian LTS and thirty-third month as a Debian ELTS paid contributor.  
I worked for XX hours for LTS and XX hours for ELTS.

#### LTS CVE Fixes and Announcements:

- Fixed CVE-2022-47016 for tmux and uploaded to buster via 2.8-3+deb10u1.  
  But decided to not roll the DLA for the package as the CVE got rejected upstream.
- Issued [DLA 3359-1](https://lists.debian.org/debian-lts-announce/2023/03/msg00010.html), fixing [CVE-2019-13038](https://security-tracker.debian.org/tracker/CVE-2019-13038) and [CVE-2021-3639](https://security-tracker.debian.org/tracker/CVE-2021-3639), for [libapache2-mod-auth-mellon](https://tracker.debian.org/pkg/libapache2-mod-auth-mellon).  
  For Debian 10 buster, these problems have been fixed in version 0.14.2-1+deb10u1.
- Issued [DLA 3360-1](https://lists.debian.org/debian-lts-announce/2023/03/msg00011.html), fixing [CVE-2021-30151](https://security-tracker.debian.org/tracker/CVE-2021-30151) and [CVE-2022-23837](https://security-tracker.debian.org/tracker/CVE-2022-23837), for [ruby-sidekiq](https://tracker.debian.org/pkg/ruby-sidekiq).  
  For Debian 10 buster, these problems have been fixed in version 5.2.3+dfsg-1+deb10u1.
- Worked on ruby-rails-html-sanitize and added notes to the security-tracker.  
  TL;DR: we need newer methods in ruby-loofah to make the patches for ruby-rails-html-sanitize backportable.
- Started to look at other set of packages meanwhile.

#### ELTS CVE Fixes and Announcements:

- Issued [ELA 813-1](), fixing [CVE-2017-12618](https://security-tracker.debian.org/tracker/CVE-2017-12618) and [CVE-2022-25147](https://security-tracker.debian.org/tracker/CVE-2022-25147), for [apr-util](https://tracker.debian.org/pkg/apr-util).  
  For Debian 8 jessie, these problems have been fixed in version 1.5.4-1+deb8u1.  
  For Debian 9 stretch, these problems have been fixed in version 1.5.4-3+deb9u1.
- Issued [ELA 814-1](), fixing [CVE-2022-39286](https://security-tracker.debian.org/tracker/CVE-2022-39286), for [jupyter-core](https://tracker.debian.org/pkg/jupyter-core).  
  For Debian 9 stretch, these problems have been fixed in version 4.2.1-1+deb9u1.
- Issued [ELA 815-1](), fixing [CVE-2022-44792](https://security-tracker.debian.org/tracker/CVE-2022-44792) and [CVE-2022-44793](https://security-tracker.debian.org/tracker/CVE-2022-44793), for [net-snmp](https://tracker.debian.org/pkg/net-snmp).  
  For Debian 8 jessie, these problems have been fixed in version 5.7.2.1+dfsg-1+deb8u6.  
  For Debian 9 stretch, these problems have been fixed in version 5.7.3+dfsg-1.7+deb9u5.
- Helped facilitate RabbitMQ's update queries by one of our customers.
- Started to look at other set of packages meanwhile.

#### Other (E)LTS Work:

- Triaged [ruby-loofah](https://tracker.debian.org/pkg/ruby-loofah),
[ruby-sinatra](https://tracker.debian.org/pkg/ruby-sinatra),
[tmux](https://tracker.debian.org/pkg/tmux),
[ruby-sidekiq](https://tracker.debian.org/pkg/ruby-sidekiq),
[libapache2-mod-auth-mellon](https://tracker.debian.org/pkg/libapache2-mod-auth-mellon),
[jupyter-core](https://tracker.debian.org/pkg/jupyter-core),
[net-snmp](https://tracker.debian.org/pkg/net-snmp), and
[apr-util](https://tracker.debian.org/pkg/apr-util),
[rabbitmq-server](https://tracker.debian.org/pkg/rabbitmq-server).
- Helped and assisted new contributors joining Freexian (LTS/ELTS/internally).
- Answered questions (& discussions) on IRC (#debian-lts and #debian-elts) and Matrix.
- Participated and helped fellow members with their queries via private mail and chat.
- General and other discussions on LTS private and [public mailing list](https://lists.debian.org/debian-lts/2023/02/threads.html).
- Attended the monthly LTS meeting.

---

Until next time.  
`:wq` for today.
