+++
date = "2023-07-30 11:11:11 +0530"
title = "FOSS Activites in July 2023"
slug = "foss-in-july-23"
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

Here's my (forty-sixth) monthly but brief update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 55th month of actively contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March 2019 and a [DD](https://wiki.debian.org/DebianDeveloper) on Christmas '19! \o/

There's a bunch of things I do, both, technical and non-technical. Here are the things I did this month:

### Uploads

- [redmine](https://tracker.debian.org/pkg/redmine) (5.0.4-7) - Add patch to let redmine run from its own user. ([debbug#1022815](https://bugs.debian.org/1022815))
- [redmine](https://tracker.debian.org/pkg/redmine) (5.0.4-5~bpo11+2) - Backporting the above changes to bullseye.

### Others

- Mentoring for newcomers.
- Sponsored matthiasmullie-minify for Athos.
- Bug work and MR review for redmine.
- Moderation of -project mailing list.
- DebConf Bursary work. Quite a month. But the bursary stuff is mostly done, we have rolled out the second batch already. About to do the final round super soon.

A huge thanks to Freexian for sponsoring my Debian work and Entrouvert for sponsoring the Redmine backports. :D

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

This was my 30th month of actively contributing to [Ubuntu](https://ubuntu.com/about).
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

This was my forty-sixth month as a Debian LTS and thirty-third month as a Debian ELTS paid contributor.  
I worked for 1.5 hours for LTS and 1.00 hours for ELTS.

#### LTS Work:

- ruby-rack v/s ruby-sinatra regression investigation. Took 30 minutes, roughly.

#### ELTS Work:

- Started to look at ruby-rack for stretch, a general triage and understanding the issue this month. Will continue to work on this and rails next month.

#### Other (E)LTS Work:

- Triaged [ruby-rack](https://tracker.debian.org/pkg/ruby-rack).
- Answered questions (& discussions) on IRC (#debian-lts and #debian-elts) and Matrix.
- Participated and helped fellow members with their queries via private mail and chat.
- General and other discussions on LTS private and [public mailing list](https://lists.debian.org/debian-lts/2023/07/threads.html).
- Attended the monthly LTS meeting.

---

Until next time.  
`:wq` for today.
