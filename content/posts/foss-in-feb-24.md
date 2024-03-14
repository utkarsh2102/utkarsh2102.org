+++
date = "2024-02-29 11:11:11 +0530"
title = "FOSS Activites in February 2024"
slug = "foss-in-feb-24"
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

Here's my (fifty-third) monthly but brief update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 62nd month of actively contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March 2019 and a [DD](https://wiki.debian.org/DebianDeveloper) on Christmas '19! \o/

There's a bunch of things I do, both, technical and non-technical. Here's what I did:

- Reviewed pyparted MR and gave feedback on the package adoption to Mitch.
- Mentoring for newcomers.
- Sponsorship of some Golang packages for Lena Voytek.
- Moderation of -project mailing list.

A huge thanks to Freexian for sponsoring my Debian work. :D

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

This was my 37th month of actively contributing to [Ubuntu](https://ubuntu.com/about).
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

This was my fifty-third month as a Debian LTS and fourtieth month as a Debian ELTS paid contributor.  
I worked for 11.25 hours for LTS and 7.25 hours for ELTS.

I did the following things:

- LTS & ELTS frontdesk from 11-12 to 17-12.
- And then a couple of days (24th and 25th), substituting Emilio.
- Triaged [composer](https://tracker.debian.org/pkg/composer),
[openvswitch](https://tracker.debian.org/pkg/openvswitch),
[zabbix](https://tracker.debian.org/pkg/zabbix),
[kde4libs](https://tracker.debian.org/pkg/kde4libs),
[zfs-linux](https://tracker.debian.org/pkg/zfs-linux),
[libgit2](https://tracker.debian.org/pkg/libgit2),
[bind9](https://tracker.debian.org/pkg/bind9),
[ckeditor](https://tracker.debian.org/pkg/ckeditor),
[ckeditor3](https://tracker.debian.org/pkg/ckeditor3),
[gpac](https://tracker.debian.org/pkg/gpac),
[389-ds-base](https://tracker.debian.org/pkg/389-ds-base),
[libxml2](https://tracker.debian.org/pkg/libxml2),
[node-yarnpkg](https://tracker.debian.org/pkg/node-yarnpkg),
[python-aiohttp](https://tracker.debian.org/pkg/python-aiohttp),
[vim](https://tracker.debian.org/pkg/vim),
[angular.js](https://tracker.debian.org/pkg/angular.js), and
[diffoscope](https://tracker.debian.org/pkg/diffoscope).
- Marked CVE-2024-24815/ckeditor3 as end-of-life for buster.
- Marked CVE-2024-24816/ckeditor3 as end-of-life for buster.
- Marked CVE-2024-2426{5,6,7}/gpac as end-of-life for buster.
- Marked ckeditor and ckeditor3 as EOL for stretch and jessie.
- Marked CVE-2024-1062/389-ds-base as no-dsa for buster.
- Marked CVE-2024-25062/libxml2 as no-dsa for buster, stretch, and jessie.
- Marked CVE-2021-4435/node-yarnpkg as no-dsa for buster.
- Marked CVE-2024-23334/python-aiohttp as no-dsa for buster.
- Marked CVE-2024-23829/python-aiohttp as no-dsa for buster.
- Marked CVE-2024-22667/vim as no-dsa for buster, stretch, and jessie.
- Marked CVE-2024-21490/angular.js as postponed for buster.
- Marked CVE-2024-25711/diffoscope as no-dsa for buster.
- Auto EOL'd webkit2gtk, libhibernate-validator-java, openvswitch, linux, engrampa, chromium, gpac, libgit2, wordpress, ckeditor, ckeditor3, firefox-esr, lucene-solr, angular.js, hugin, diffoscope, ruby-rack, and nodejs.
- Reviewed man-db update for Colin; cf: https://lists.debian.org/debian-lts/2024/02/msg00000.html.
- Helped facilitate Firefox and Thunderbird DLA for Emilio. However, most of the time was spent in making sure the builds were successful and that there are binaries available for users.
- Understood Thunderbird's situation and history of its armhf builds; cf: https://lists.debian.org/debian-lts/2024/02/msg00021.html.
- Worked on some packages, like zfs-linux, kde4libs, and libgit2 but couldn't complete them. Will get back to it next month.
- Answered questions (& discussions) on IRC (#debian-lts and #debian-elts) and Matrix.
- Participated and helped fellow members with their queries.
- General and other discussions on LTS private and [public mailing list](https://lists.debian.org/debian-lts/2024/02/threads.html).
- Attended the monthly LTS meeting.

---

Until next time.  
`:wq` for today.
