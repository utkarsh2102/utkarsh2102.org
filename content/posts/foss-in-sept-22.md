+++
date = "2022-09-30 11:11:11 +0530"
title = "FOSS Activites in September 2022"
slug = "foss-in-sept-22"
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

Here's my (thirty-sixth) monthly but brief update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 45th month of actively contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March 2019 and a [DD](https://wiki.debian.org/DebianDeveloper) on Christmas '19! \o/

There's a bunch of things I do, both, technical and non-technical. Here are the things I did this month:

#### Debian Uploads

- [rails](https://tracker.debian.org/pkg/rails) (2:6.1.6.1+dfsg-2) - Add patch to allow Symbols in YAML columns, fixes [#1018934](https://bugs.debian.org/1018934).
- [rails](https://tracker.debian.org/pkg/rails) (2:6.1.6.1+dfsg-3) - Add patch to remove active_record.yaml initializers.
- [rails](https://tracker.debian.org/pkg/rails) (2:6.1.6.1+dfsg-4) - Add patch to allow Date, Time, ActiveSupport::HashWithIndifferentAccess in YAML columns.
- [ruby-arbre](https://tracker.debian.org/pkg/ruby-arbre) (1.4.0-2) - Add patch to use selector to detect authenticity token input.
- [ruby-net-http-digest-auth](https://tracker.debian.org/pkg/ruby-net-http-digest-auth) (1.4.1-1) - New upstream version, v1.4.1 to fix the FTBFS w/ rails.
- [rails](https://tracker.debian.org/pkg/rails) (2:6.1.7+dfsg-1) - New upstream version, v6.1.7+dfsg.
- [redmine](https://tracker.debian.org/pkg/redmine) (5.0.2-1) - New upstream version, v5.0.2 + fixes for [#1017525](https://bugs.debian.org/1017525), [#1019607](https://bugs.debian.org/1019607), [#1019238](https://bugs.debian.org/1019238), and [#1014813](https://bugs.debian.org/1014813).
- [redmine](https://tracker.debian.org/pkg/redmine) (5.0.2-2) - Add patch to relax pg's version for autopkgtest.
- [ruby-json-jwt](https://tracker.debian.org/pkg/ruby-json-jwt) (1.14.0-2) - No-change rebuild for unstable to fix [#1011682](https://bugs.debian.org/1011682).
- [libexporter-tiny-perl](https://tracker.debian.org/pkg/libexporter-tiny-perl) (1.004002-1) - New upstream version, v1.004002.

#### Other $things:

- Sponsored php-nikic-fast-route/1.3.0-4~bpo11+1 for William.
- Being an AM for [Arun Kumar, process #1024](https://nm.debian.org/process/1024/).
- Sponsoring stuff for non-DDs.
- Mentoring for newcomers.
- Moderation of -project mailing list.

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

This was my 20th month of actively contributing to [Ubuntu](https://ubuntu.com/about).
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

This was my thirty-sixth month as a Debian LTS and twenty-seventh month as a Debian ELTS paid contributor.  
I worked for 38.00 hours for LTS and 27.00 hours for ELTS.

#### LTS CVE Fixes and Announcements:


#### ELTS CVE Fixes and Announcements:


#### Other (E)LTS Work:

- Triaged [cifs-utils](https://tracker.debian.org/pkg/cifs-utils),
[lrzip](https://tracker.debian.org/pkg/lrzip), and
[mutt](https://tracker.debian.org/pkg/mutt).
- Helped and assisted new contributors joining Freexian (LTS/ELTS).
- Answered questions (& discussions) on IRC (#debian-lts and #debian-elts) and Matrix.
- Participated and helped fellow members with their queries via private mail and chat.
- General and other discussions on LTS private and [public mailing list](https://lists.debian.org/debian-lts/2022/09/threads.html).
- Attended the monthly public meeting held on #debian-lts on September 29th.


---

Until next time.  
`:wq` for today.
