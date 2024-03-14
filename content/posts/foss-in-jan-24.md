+++
date = "2024-01-30 11:11:11 +0530"
title = "FOSS Activites in January 2024"
slug = "foss-in-jan-24"
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

Here's my (fifty-second) monthly but brief update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 61st month of actively contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March 2019 and a [DD](https://wiki.debian.org/DebianDeveloper) on Christmas '19! \o/

There's a bunch of things I do, both, technical and non-technical. Here's what I did:

- Some sync up w/ DC24 team, gearing up for DC24 prep. \o/
- Mentoring for newcomers.
- Sponsorship of some Golang packages for Lena Voytek.
- Moderation of -project mailing list.

A huge thanks to Freexian for sponsoring my Debian work. :D

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

This was my 36th month of actively contributing to [Ubuntu](https://ubuntu.com/about).
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

This was my fifty-second month as a Debian LTS and thirty-ninth month as a Debian ELTS paid contributor.  
I worked for 8.50 hours for LTS and 8.00 hours for ELTS.

I did the following things:

- Triaged [keystone](https://tracker.debian.org/pkg/keystone),
[rails](https://tracker.debian.org/pkg/rails),
[inetutils](https://tracker.debian.org/pkg/inetutils),
[kde4libs](https://tracker.debian.org/pkg/kde4libs), and
[zfs-linux](https://tracker.debian.org/pkg/zfs-linux).
- Worked on zfs-linux and kde4libs partly. DLA and ELA to go out soon. Sadly I couldn't finish it to completion.
- Uploaded inetutils to jessie, fixing 4 CVEs. This is a newly supported package and so we decided to issue an update for jessie.
  The same CVEs are fixed in other suites, however.
- Discussed the situation of rails in buster with Santiago, as buster will soon be ELTS, we'd like to ensure it's something that we can provide support for.
- Answered questions (& discussions) on IRC (#debian-lts and #debian-elts) and Matrix.
- Participated and helped fellow members with their queries.
- General and other discussions on LTS private and [public mailing list](https://lists.debian.org/debian-lts/2023/12/threads.html).
- Attended the monthly LTS meeting.

---

Until next time.  
`:wq` for today.
