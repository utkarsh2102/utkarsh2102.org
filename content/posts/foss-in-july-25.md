+++
date = "2025-07-30 11:11:11 +0530"
title = "FOSS Activites in July 2025"
slug = "foss-in-july-25"
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

Here's my 70th monthly but brief update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 79th month of actively contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March 2019 and a [DD](https://wiki.debian.org/DebianDeveloper) on Christmas '19! \o/

Debian was in freeze throughout so whilst I didn't do many uploads, there's a bunch of other things I did:

- Attended DebConf25 in Brest, France.
  - Lead the bursary BOF and discussions.
  - Participated in other sessions, especially around the FTP masters.
  - I've started to look at things with my trainee hat on.
  - Participated in the Debian Security Tracker sprints during DebCamp. More on that below.
- Mentoring for newcomers.
- Moderation of -project mailing list.

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

This was my 54th month of actively contributing to [Ubuntu](https://ubuntu.com/about).
I joined [Canonical to work on Ubuntu full-time](https://utkarsh2102.org/posts/hello-canonical/) back in February 2021.

Whilst I can't give a full, detailed list of things I did (there's so much and some of it might not be public...yet!), here's a quick TL;DR of what I did:

- [Released Questing snapshot 3](https://discourse.ubuntu.com/t/questing-snapshot-3-released/65383)! \o/
- [EOL'd Oracular](https://discourse.ubuntu.com/t/ubuntu-24-10-oracular-oriole-reached-end-of-life-on-10th-july-2025/64289). o/
- Participated in the mid-cycle sprints.
- Got a recognition award for leading 24.04.2 LTS release and leading the Release Management team.
- Preparing for the 24.04.3 LTS release early next month.

---

## Debian (E)LTS
{{< figure src="/images/debian-lts-small.png" >}}

[Debian Long Term Support (LTS)](https://www.freexian.com/en/services/debian-lts.html) is a project to extend the lifetime of all Debian stable releases to (at least) 5 years. Debian LTS is not handled by the Debian security team, but by a separate group of volunteers and companies interested in making it a success.  

And [Debian Extended LTS (ELTS)](https://deb.freexian.com/extended-lts) is its sister project, extending support to the stretch and jessie release (+2 years after LTS support).

This was my 70th month as a Debian LTS and 57th month as a Debian ELTS paid contributor.  
I only worked for 15.00 hours for LTS and 5.00 hours for ELTS and did the following things:

- [LTS] Released [DLA 4263-1](https://lists.debian.org/debian-lts-announce/2025/08/msg00002.html) for ruby-graphql.
  - Coordinated with upstream due to lack of clarity on 1.11.4 being affected & not having a clear reproducer.
  - As 1.11.4 was still partially vulnerable and the backport was non-trivial, it was probably conveinent to bump the upstream version to 1.11.12 instead, fixing:
  - [CVE-2025-27407)](https://security-tracker.debian.org/tracker/CVE-2025-27407): a remote code execution.
  - Salsa repository: https://salsa.debian.org/lts-team/packages/ruby-graphql.
  - Coordinated with the Security team for a p-u fix or a DSA.
- [E/LTS] Frontdesk duty from 28th July to 04th August.
  - Triaged a bunch of CVEs.
  - Raised an inconsistency about [issues being fixed in buster & bookworm but not in bullseye](https://lists.debian.org/debian-lts/2025/07/msg00017.html).
  - Helped Bastien with ca-certificates bit & coordinating with fellow Debian contributors.
  - Also triaged some newly supported packages for ELTS.
- [LTS] Attended the monthly LTS meeting on IRC. [Summary here](https://meetbot.debian.net/debian-lts/2025/debian-lts.2025-07-24-14.00.html).

### Debian Security Tracker sprint 2025

Thanks to the LTS team for also organizing a security tracker sprint during DebCamp25. I attended the sprint and spent 10 hours working on the following tasks:

- JSON API documentation:
  - Issue: https://salsa.debian.org/security-tracker-team/security-tracker/-/issues/15
  - MR: https://salsa.debian.org/security-tracker-team/security-tracker/-/merge_requests/237
  - This also includes actioning of Roberto's and Salvatore's review.

- Missing -1 from DSA entries causing web redirects to fail:
  - Issue: https://salsa.debian.org/security-tracker-team/security-tracker/-/issues/28
  - MR: https://salsa.debian.org/security-tracker-team/security-tracker/-/merge_requests/224
  - This includes some coordination with the web team and some back and forth with them to ensure both the Web team and the Security team would be happy with the fix. It also fixes more issues as mentioned in the description of the MR.

- Show packages from next-point-release.txt in source package overview
  - Bug: https://bugs.debian.org/cgi-bin/bugreport.cgi?bug=989065
  - Did some initial brainstorming on the issue, haven't had time to do the actual implementation.
  - I intend to continue working on it as time allows in the next weeks & months. Will update if & when I make progress.

That's all. A quicky shoutout to Roberto for organizing the sprints remotely and being awake at odd hours. <3


---

Until next time.  
`:wq` for today.
