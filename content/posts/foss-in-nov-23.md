+++
date = "2023-11-30 11:11:11 +0530"
title = "FOSS Activites in November 2023"
slug = "foss-in-nov-23"
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

Here's my (fiftieth) monthly but brief update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 59th month of actively contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March 2019 and a [DD](https://wiki.debian.org/DebianDeveloper) on Christmas '19! \o/

There's a bunch of things I do, both, technical and non-technical. Here's what I did:

- Helped w/ /usr-merge (DEP 17) work and fixed 3 packages: net-tools, gitlab, and libnfc.
- Attended MiniDebCamp and MiniDebConf Cambridge. Super fun hanging out w/ Debainites.
- Sponsored django-assets, python-django-tagging, and django-menu-generator-ng for Lena Voytek.
- Reviewed django-dbbackup for Lena. Couldn't sponsor as it FTBFS.
- Mentoring for newcomers.
- Moderation of -project mailing list.

A huge thanks to Freexian for sponsoring my Debian work. :D

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

This was my 34th month of actively contributing to [Ubuntu](https://ubuntu.com/about).
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

This was my fiftieth month as a Debian LTS and thirty-seventh month as a Debian ELTS paid contributor.  
I worked for 4.75 hours for LTS and 11.00 hours for ELTS.

I did the following things:

- ELTS frontdesk from 20-11 to 26-11.
- Marked CVE-2022-46337/derby as postponed for stretch.
- Marked CVE-2023-48161/giflib as no-dsa for stretch and jessie; following buster.
- Marked CVE-2023-47038/perl as not-affected for stretch and jessie.
- Auto EOL'd capnproto, gpac, radare2, minizip, gimp-dds, libde265, strongswan, cargo, bouncycastle, linux, firefox-esr, thunderbird, gnutls28, and derby.
- Noticed and pinged Bastien about the missing ceph/0.80.7-2+deb8u6 upload to jessie.
- Figured what's wrong with ruby-rmagick autopkgtest in jessie; it's a bug in autopkgtest/debci.
- Pinged Adrian about fixing CVEs fixed via ELA-909-1/DLA-3513-1 in (old)stable.
- Worked on strongswan for jessie with Chris Lamb together during MiniDebConf Cambridge.
- Partook in various discussions about ELTS packages and their support w/ Santiago and Roberto, and others, during the Freexian sprints.
- Prepared distro-info-data update with LTS/ELTS EOL dates and uploaded it to unstable. Will prep it for stable, LTS, and ELTS in coordination w/ Stefano.
- Let my colleagues know about my whereabouts in the last few months.
- Answered questions (& discussions) on IRC (#debian-lts and #debian-elts) and Matrix.
- Participated and helped fellow members with their queries.
- General and other discussions on LTS private and [public mailing list](https://lists.debian.org/debian-lts/2023/10/threads.html).
- Attended the monthly LTS meeting.

---

Until next time.  
`:wq` for today.
