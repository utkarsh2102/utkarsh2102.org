+++
date = "2023-01-30 11:11:11 +0530"
title = "FOSS Activites in January 2023"
slug = "foss-in-jan-23"
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

Here's my (fortieth) monthly but brief update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 49th month of actively contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March 2019 and a [DD](https://wiki.debian.org/DebianDeveloper) on Christmas '19! \o/

There's a bunch of things I do, both, technical and non-technical. Here are the things I did this month:

### Uploads

- [redmine](https://tracker.debian.org/pkg/redmine) (5.0.4-1) - Fixing bug #1022818, #1026048, and #1027340.
- [libyang2](https://tracker.debian.org/pkg/libyang2) (2.1.30-2) - Adding DEP8 test for yangre.

### Others

- Proposed tomcat9 bullseye -pu via 9.0.43-2~deb11u5.
- Helped Otto with review of mariadb from NEW.
- Sponsored php-font-lib for William.
- Advocated William for becoming DD, uploading.
- Granted some DM rights.
- Mentoring for newcomers.
- Reviewed libgit2 bits, new uploads and changes.
- Moderation of -project mailing list.

A huge thanks to Freexian for sponsoring my Debian work. :D

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

This was my 24th month of actively contributing to [Ubuntu](https://ubuntu.com/about).
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

This was my fortieth month as a Debian LTS and thirty-first month as a Debian ELTS paid contributor.  
I worked for 43.25 hours for LTS and 25.00 hours for ELTS.

#### LTS CVE Fixes and Announcements:

- Issued [DLA 3281-1](https://lists.debian.org/debian-lts-announce/2023/01/msg00021.html), fixing [CVE-2022-47950](https://security-tracker.debian.org/tracker/CVE-2022-47950), for [swift](https://tracker.debian.org/pkg/swift).  
  For Debian 10 buster, these problems have been fixed in version 2.19.1-1+deb10u1.
- Issued [DLA 3295-1](https://lists.debian.org/debian-lts-announce/2023/01/msg00035.html), fixing [CVE-2022-24785](https://security-tracker.debian.org/tracker/CVE-2022-24785) and [CVE-2022-31129](https://security-tracker.debian.org/tracker/CVE-2022-31129), for [node-moment](https://tracker.debian.org/pkg/node-moment).  
  For Debian 10 buster, these problems have been fixed in version 2.24.0+ds-1+deb10u1.
- Issued [DLA 3296-1](https://lists.debian.org/debian-lts-announce/2023/01/msg00036.html), fixing [CVE-2023-24038](https://security-tracker.debian.org/tracker/CVE-2023-24038), for [libhtml-stripscripts-perl](https://tracker.debian.org/pkg/libhtml-stripscripts-perl).  
  For Debian 10 buster, these problems have been fixed in version 1.06-1+deb10u1.
- Issued [DLA 3297-1](https://lists.debian.org/debian-lts-announce/2023/01/msg00037.html), fixing [CVE-2022-48281](https://security-tracker.debian.org/tracker/CVE-2022-48281), for [tiff](https://tracker.debian.org/pkg/tiff).  
  For Debian 10 buster, these problems have been fixed in version 4.1.0+git191117-2~deb10u6.
- Issued [DLA 3298-1](https://lists.debian.org/debian-lts-announce/2023/01/msg00038.html), fixing [CVE-2020-8161](https://security-tracker.debian.org/tracker/CVE-2020-8161), [CVE-2020-8184](https://security-tracker.debian.org/tracker/CVE-2020-8184), [CVE-2022-44570](https://security-tracker.debian.org/tracker/CVE-2022-44570), [CVE-2022-44571](https://security-tracker.debian.org/tracker/CVE-2022-44571), and [CVE-2022-44572](https://security-tracker.debian.org/tracker/CVE-2022-44572), for [ruby-rack](https://tracker.debian.org/pkg/ruby-rack).  
  For Debian 10 buster, these problems have been fixed in version 2.0.6-3+deb10u2.
- Issued [DLA 3300-1](https://lists.debian.org/debian-lts-announce/2023/01/msg00040.html), fixing [CVE-2022-47951](https://security-tracker.debian.org/tracker/CVE-2022-47951), for [glance](https://tracker.debian.org/pkg/glance).  
  For Debian 10 buster, these problems have been fixed in version 2:17.0.0-5+deb10u1.
- Issued [DLA 3301-1](https://lists.debian.org/debian-lts-announce/2023/01/msg00041.html), fixing [CVE-2022-47951](https://security-tracker.debian.org/tracker/CVE-2022-47951), for [cinder](https://tracker.debian.org/pkg/cinder).  
  For Debian 10 buster, these problems have been fixed in version 2:13.0.7-1+deb10u2.
- Issued [DLA 3302-1](https://lists.debian.org/debian-lts-announce/2023/01/msg00042.html), fixing [CVE-2022-47951](https://security-tracker.debian.org/tracker/CVE-2022-47951), for [nova](https://tracker.debian.org/pkg/nova).  
  For Debian 10 buster, these problems have been fixed in version 2:18.1.0-6+deb10u2.
- Issued [DLA 3303-1](https://lists.debian.org/debian-lts-announce/2023/01/msg00043.html), fixing [CVE-2022-25648](https://security-tracker.debian.org/tracker/CVE-2022-25648), [CVE-2022-46648](https://security-tracker.debian.org/tracker/CVE-2022-46648), and [CVE-2022-47318](https://security-tracker.debian.org/tracker/CVE-2022-47318), for [ruby-git](https://tracker.debian.org/pkg/ruby-git).  
  For Debian 10 buster, these problems have been fixed in version 1.2.8-1+deb10u1.
- Started to look at other set of packages.

#### ELTS CVE Fixes and Announcements:

- Issued [ELA 784-1](https://www.freexian.com/lts/extended/updates/ela-784-1-ruby-git/), fixing [CVE-2022-25648](https://security-tracker.debian.org/tracker/CVE-2022-25648), [CVE-2022-46648](https://security-tracker.debian.org/tracker/CVE-2022-46648), and [CVE-2022-47318](https://security-tracker.debian.org/tracker/CVE-2022-47318), for [ruby-git](https://tracker.debian.org/pkg/ruby-git).  
  For Debian 9 stretch, these problems have been fixed in version 1.2.8-1+deb9u1.
- Issued [ELA 785-1](https://www.freexian.com/lts/extended/updates/ela-785-1-ruby-rack/), fixing [CVE-2022-44570](https://security-tracker.debian.org/tracker/CVE-2022-44570) and [CVE-2022-44571](https://security-tracker.debian.org/tracker/CVE-2022-44571), for [ruby-rack](https://tracker.debian.org/pkg/ruby-rack).  
  For Debian 9 stretch, these problems have been fixed in version 1.6.4-4+deb9u4.
- Issued [ELA 787-1](https://www.freexian.com/lts/extended/updates/ela-787-1-ruby-sinatra/), fixing [CVE-2022-45442](https://security-tracker.debian.org/tracker/CVE-2022-45442), for [ruby-sinatra](https://tracker.debian.org/pkg/ruby-sinatra).  
  For Debian 9 stretch, these problems have been fixed in version 1.4.7-5+deb9u2.
- Helped facilitate Erlang's and RabbitMQ's update; cf: [ELA 754-1](https://www.freexian.com/lts/extended/updates/ela-754-1-erlang/).
- Started to look at other set of packages.

#### Other (E)LTS Work:

- Triaged [node-moment](https://tracker.debian.org/pkg/node-moment),
[modsecurity-apache](https://tracker.debian.org/pkg/modsecurity-apache),
[ruby-git](https://tracker.debian.org/pkg/ruby-git),
[ruby-sinatra](https://tracker.debian.org/pkg/ruby-sinatra),
[gpac](https://tracker.debian.org/pkg/gpac),
[cargo](https://tracker.debian.org/pkg/cargo),
[git](https://tracker.debian.org/pkg/git),
[openjdk-11](https://tracker.debian.org/pkg/openjdk-11),
[swift](https://tracker.debian.org/pkg/swift),
[libxpm](https://tracker.debian.org/pkg/libxpm),
[lilypond](https://tracker.debian.org/pkg/lilypond),
[openjdk-8](https://tracker.debian.org/pkg/openjdk-8),
[modsecurity](https://tracker.debian.org/pkg/modsecurity),
[netdata](https://tracker.debian.org/pkg/netdata),
[nim](https://tracker.debian.org/pkg/nim),
[rust-cargo](https://tracker.debian.org/pkg/rust-cargo),
[sgt-puzzles](https://tracker.debian.org/pkg/sgt-puzzles),
[apache2](https://tracker.debian.org/pkg/apache2),
[wireshark](https://tracker.debian.org/pkg/wireshark),
[libhtml-stripscripts-perl](https://tracker.debian.org/pkg/libhtml-stripscripts-perl),
[redis](https://tracker.debian.org/pkg/redis),
[tomcat8](https://tracker.debian.org/pkg/tomcat8),
[tiff](https://tracker.debian.org/pkg/tiff),
[ruby-rack](https://tracker.debian.org/pkg/ruby-rack),
[tmux](https://tracker.debian.org/pkg/tmux),
[ruby-rack](https://tracker.debian.org/pkg/ruby-rack),
[ruby-sidekiq](https://tracker.debian.org/pkg/ruby-sidekiq),
[libapache2-mod-auth-mellon](https://tracker.debian.org/pkg/libapache2-mod-auth-mellon),
[jupyter-core](https://tracker.debian.org/pkg/jupyter-core),
[net-snmp](https://tracker.debian.org/pkg/net-snmp), and
[rabbitmq-server](https://tracker.debian.org/pkg/rabbitmq-server).
- Marked CVE-2023-{0358,2314{3-5}}/gpac as EOL for buster.
- Marked CVE-2022-46176/cargo as no-dsa in buster.
- Marked CVE-2022-4{4617,6285,883}/libxpm as no-dsa for buster, stretch, and jessie.
- Marked CVE-2020-17354/lilypond as ignored for buster.
- Marked CVE-2022-48279/modsecurity as no-dsa for buster.
- Marked CVE-2023-2249{6,7}/netdata as no-dsa for buster.
- Marked CVE-2021-46872/nim as no-dsa for buster.
- Marked CVE-2022-46176/rust-cargo as no-dsa in buster.
- Marked TEMP-1028986-7037E6/sgt-puzzles as no-dsa for buster.
- Marked CVE-2006-20001 and CVE-2022-3{6760,7436}/apache2 as postponed for stretch and jessie.
- Marked CVE-2023-22458/redis as not-affected for stretch and jessie.
- Marked CVE-2022-45143/tomcat8 as postponed for stretch and jessie.
- Marked CVE-2022-44572/ruby-rack as not-affected for stretch.
- Marked CVE-2022-47950/swift as not-affected for stretch.
- Auto EOL'd node-debug, nim, netty, ruby-git, firefox-esr, linux, swift, radare2, gpac, virtualbox, shiro, sgt-puzzles, pdns-recursor, sofia-sip, libgit2, wireshark, amanda, libhtml-stripscripts-perl, pkgconf, libapache-session-ldap-perl, golang-yaml.v2, nvidia-graphics-drivers, xen, rails, ruby-rack, assimp, thunderbird, cinder, glance, nova, editorconfig-core, chromium, ruby-globalid, spip, opusfile, pgpool2, and ruby-sanitize.
- Helped and assisted new contributors joining Freexian (LTS/ELTS/internally).
- Answered questions (& discussions) on IRC (#debian-lts and #debian-elts) and Matrix.
- Participated and helped fellow members with their queries via private mail and chat.
- General and other discussions on LTS private and [public mailing list](https://lists.debian.org/debian-lts/2023/01/threads.html).
- Attended the monthly LTS meeting.

---

Until next time.  
`:wq` for today.
