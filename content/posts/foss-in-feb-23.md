+++
date = "2023-02-28 11:11:11 +0530"
title = "FOSS Activites in February 2023"
slug = "foss-in-feb-23"
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

Here's my (forty-first) monthly but brief update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 50th month of actively contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March 2019 and a [DD](https://wiki.debian.org/DebianDeveloper) on Christmas '19! \o/

There's a bunch of things I do, both, technical and non-technical. Here are the things I did this month:

### Uploads

- [ruby-delayed-job](https://tracker.debian.org/pkg/ruby-delayed-job) (4.1.9-1~bpo11+1) - Backport to bullseye.
- [ruby-delayed-job-active-record](https://tracker.debian.org/pkg/ruby-delayed-job-active-record) (4.1.6-3~bpo11+1) - Backport to bullseye.
- [ruby-globalid](https://tracker.debian.org/pkg/ruby-globalid) (0.6.0-1~bpo11+1) - Backport to bullseye.
- [ruby-tzinfo](https://tracker.debian.org/pkg/ruby-tzinfo) (2.0.4-1~bpo11+2) - Backport to bullseye.
- [rails](https://tracker.debian.org/pkg/rails) (2:6.1.7+dfsg-3~bpo11+1) - Backport to bullseye.
- [ruby-commonmarker](https://tracker.debian.org/pkg/ruby-commonmarker) (0.23.6-1~bpo11+1) - Backport to bullseye.
- [ruby-csv](https://tracker.debian.org/pkg/ruby-csv) (3.2.2-1~bpo11+1) - Backport to bullseye.
- [ruby-task-list](https://tracker.debian.org/pkg/ruby-task-list) (2.3.2-2~bpo11+1) - Backport to bullseye.
- [ruby-i18n](https://tracker.debian.org/pkg/ruby-i18n) (1.10.0-2~bpo11+1) - Backport to bullseye.
- [ruby-mini-magick](https://tracker.debian.org/pkg/ruby-mini-magick) (4.11.0-1~bpo11+1) - Backport to bullseye.
- [ruby-net-ldap](https://tracker.debian.org/pkg/ruby-net-ldap) (0.17.0-1~bpo11+1) - Backport to bullseye.
- [ruby-roadie-rails](https://tracker.debian.org/pkg/ruby-roadie-rails) (3.0.0-1~bpo11+1) - Backport to bullseye.
- [ruby-roadie](https://tracker.debian.org/pkg/ruby-roadie) (5.1.0-1~bpo11+1) - Backport to bullseye.
- [ruby-sanitize](https://tracker.debian.org/pkg/ruby-sanitize) (6.0.0-1~bpo11+1) - Backport to bullseye.
- [ruby-nokogiri](https://tracker.debian.org/pkg/ruby-nokogiri) (1.13.1+dfsg-2~bpo11+1) - Backport to bullseye.
- [ruby-mini-portile2](https://tracker.debian.org/pkg/ruby-mini-portile2) (2.8.0-1~bpo11+2) - Backport to bullseye.
- [ruby-webrick](https://tracker.debian.org/pkg/ruby-webrick) (1.7.0-3~bpo11+2) - Backport to bullseye.
- [ruby-zip](https://tracker.debian.org/pkg/ruby-zip) (2.3.0-2~bpo11+1) - Backport to bullseye.
- [gem2deb](https://tracker.debian.org/pkg/gem2deb) (2.1~bpo11+1) - Backport to bullseye.
- [ruby-actionpack-action-caching](https://tracker.debian.org/pkg/ruby-actionpack-action-caching) (1.2.2-1~bpo11+1) - Backport to bullseye.
- [ruby-nokogiri](https://tracker.debian.org/pkg/ruby-nokogiri) (1.13.5+dfsg-2~bpo11+1) - Backport to bullseye.
- [redmine](https://tracker.debian.org/pkg/redmine) (5.0.4-2~bpo11+1) - Backport to bullseye.
- [rails](https://tracker.debian.org/pkg/rails) (2:6.1.7+dfsg-3~bpo11+2) - Backport to bullseye.
- [ruby-roadie-rails](https://tracker.debian.org/pkg/ruby-roadie-rails) (3.0.0-1~bpo11+2) - Backport to bullseye.
- [redmine](https://tracker.debian.org/pkg/redmine) (5.0.4-4~bpo11+1) - Backport to bullseye.
- [redmine](https://tracker.debian.org/pkg/redmine) (5.0.4-5~bpo11+1) - Backport to bullseye.
- [ruby-web-console](https://tracker.debian.org/pkg/ruby-web-console) (4.2.0-1~bpo11+1) - Backport to bullseye.
- [libyang2](https://tracker.debian.org/pkg/libyang2) (2.1.30-2) - Adding DEP8 test for yangre.
- [redmine](https://tracker.debian.org/pkg/redmine) (5.0.4-3) - Add patch to stop unnecessary recursive chown'ing (Fixes: #1022816, #1022817).
- [redmine](https://tracker.debian.org/pkg/redmine) (5.0.4-4) - Set DH_RUBY_IGNORE_TESTS to all (Fixes: #1031308).
- [python-jira](https://tracker.debian.org/pkg/python-jira) (3.4.1-1) - New upstream version, v3.4.1.

### Others

- Looked up some Release team documentation.
- Sponsored php-font-lib and php-dompdf-svg-lib for William.
- Granted DM rights for php-dompdf.
- Mentoring for newcomers.
- Reviewed micro bits for Nilesh, new uploads and changes.
- Ruby sprints.
- Bug work (on BTS and #debian-ruby) for rails and redmine.
- Moderation of -project mailing list.

A huge thanks to Freexian for sponsoring my Debian work and Entrouvert for sponsoring the Redmine backports. :D

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

This was my 25th month of actively contributing to [Ubuntu](https://ubuntu.com/about).
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

This was my forty-first month as a Debian LTS and thirty-second month as a Debian ELTS paid contributor.  
I worked for 24.25 hours for LTS and 28.50 hours for ELTS.

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
