+++
date = "2024-03-30 11:11:11 +0530"
title = "FOSS Activites in March 2024"
slug = "foss-in-march-24"
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

Here's my (fifty-fourth) monthly but brief update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 63rd month of actively contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March 2019 and a [DD](https://wiki.debian.org/DebianDeveloper) on Christmas '19! \o/

There's a bunch of things I do, both, technical and non-technical. Here's what I did:

- Reviewed and sponsored some Golang packages for Lena Voytek and helped Rajudev w/ some packaging.
- Helped Mitchell Dzurick w/ the adoption of pyparted package.
- Mentoring for newcomers.
- Moderation of -project mailing list.

A huge thanks to Freexian for sponsoring my Debian work. :D

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

This was my 38th month of actively contributing to [Ubuntu](https://ubuntu.com/about).
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

This was my fifty-fourth month as a Debian LTS and fourty-first month as a Debian ELTS paid contributor.  
I worked for 19.50 hours for LTS and 17.00 hours for ELTS.

I did the following things:

- LTS & ELTS frontdesk from 25-03 to 31-03.
- Triaged [composer](https://tracker.debian.org/pkg/composer),
[node-yarnpkg](https://tracker.debian.org/pkg/node-yarnpkg),
[python-aiohttp](https://tracker.debian.org/pkg/python-aiohttp),
[atril](https://tracker.debian.org/pkg/atril),
[inetutils](https://tracker.debian.org/pkg/inetutils),
[kde4libs](https://tracker.debian.org/pkg/kde4libs),
[zfs-linux](https://tracker.debian.org/pkg/zfs-linux),
[zabbix](https://tracker.debian.org/pkg/zabbix),
[phpmyadmin](https://tracker.debian.org/pkg/phpmyadmin),
[vim](https://tracker.debian.org/pkg/vim),
[angular.js](https://tracker.debian.org/pkg/angular.js), and
[diffoscope](https://tracker.debian.org/pkg/diffoscope).
- Marked CVE-2022-48522/perl as not-affected for stretch and jessie.
- Auto EOL'd linux, webkit2gtk, minidlna, ruby-carrierwave, chromium, wireshark, composer, ampache, qtbase-opensource-src, anope, org-mode, pcp, and tinymce.
- On a support request from one of our customers, I further triaged 17 CVEs amongst 9 packages and assisting them with other queries.
- Released [ELA-1057-1](https://www.freexian.com/lts/extended/updates/ela-1057-1-inetutils/) for inetutils.
- Released [ELA-1058-1](https://www.freexian.com/lts/extended/updates/ela-1058-1-kde4libs/) for kde4libs.
- Released [DLA-3766-1](https://lists.debian.org/debian-lts-announce/2024/03/msg00019.html) for zfs-linux.
- Debugged the xz backdoor compromise issue to ensure LTS/ELTS is not affected. PS: it's not. :)
- Worked on phpmyadmin, zabbix, and atril but couldn't complete them. Will get back to it next month.
- Answered questions (& discussions) on IRC (#debian-lts and #debian-elts) and Matrix.
- Participated and helped fellow members with their queries.
- General and other discussions on LTS private and [public mailing list](https://lists.debian.org/debian-lts/2024/03/threads.html).
- Attended the monthly LTS meeting.

---

Until next time.  
`:wq` for today.
