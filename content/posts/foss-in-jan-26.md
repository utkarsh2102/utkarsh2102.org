+++
date = "2025-01-30 11:11:11 +0530"
title = "FOSS Activites in January 2026"
slug = "foss-in-jan-26"
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

Here's my monthly but brief update about the activities I've done in the FOSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

Whilst I didn't get a chance to do much, here are still a few things that I worked on:

- A few discussions with the new DFSG team, et al.
- Assited a few folks in getting their patches submitted via Salsa.
- Reviewing pyenv MR for Ujjwal.
- Mentoring for newcomers.
- Moderation of -project mailing list.

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

I joined [Canonical to work on Ubuntu full-time](https://utkarsh2102.org/posts/hello-canonical/) back in February 2021.

Whilst I can't give a full, detailed list of things I did, here's a quick TL;DR of what I did:

- Successfully released [Resolute Snapshot 3](https://discourse.ubuntu.com/t/resolute-snapshot-3-released/75832)!
  - This one was also done without the ISO tracker and cdimage access.
  - We also worked very hard to build and promote all the image in due time.
- Worked further on the whole artifact signing story for cdimage.
- Assisted a bunch of folks with my Archive Admin and Release team hats to:
  - Helped in [EOL'ing Plucky](https://discourse.ubuntu.com/t/ubuntu-25-04-plucky-puffin-reached-end-of-life-on-15th-january-2026/75079).
  - Starting to help with the upcoming 24.04.4 release.
- With that, the mid-cycle sprints are around the corner, so quite busy preparing for that.

---

## Debian (E)LTS
{{< figure src="/images/debian-lts-small.png" >}}

This month I have worked 59 hours
on [Debian Long Term Support (LTS)](https://www.freexian.com/lts/debian/)
and on its sister [Extended LTS](https://www.freexian.com/lts/extended/)
project and did the following things:

### Released Security Updates

- **adminer**: Server-side request forgery and redirection vulnerabilities in HTTP drivers.
  - **[ELTS]**: Fixed [CVE-2023-45195](https://security-tracker.debian.org/tracker/CVE-2023-45195) and [CVE-2023-45196](https://security-tracker.debian.org/tracker/CVE-2023-45196) via **4.7.1-1+deb10u2** for buster. This has been released as [**ELA 1605-1**](https://www.freexian.com/lts/extended/updates/ela-1605-1-adminer/).

- **u-boot**: Improper sanity checks in FAT filesystem handling.
  - **[ELTS]**: Fixed [CVE-2025-24857](https://security-tracker.debian.org/tracker/CVE-2025-24857) via **2016.11+dfsg1-4+deb9u2** for stretch. This has been released as [**ELA 1608-1**](https://www.freexian.com/lts/extended/updates/ela-1608-1-u-boot/).

- **ruby-rmagick**: Memory leak in Magick::Draw with ImageMagick 6.
  - **[LTS]**: Fixed [CVE-2023-5349](https://security-tracker.debian.org/tracker/CVE-2023-5349) via [**2.16.0-7+deb11u1**](https://tracker.debian.org/news/1703886/accepted-ruby-rmagick-2160-7deb11u1-source-into-oldoldstable-security/) for bullseye. This has been released as [**DLA 4433-1**](https://www.debian.org/lts/security/2025/DLA-4433-1).

- **libsodium**: Invalid point validation in Ed25519 implementation.
  - **[LTS]**: Fixed [CVE-2025-69277](https://security-tracker.debian.org/tracker/CVE-2025-69277) via [**1.0.18-1+deb11u1**](https://tracker.debian.org/news/1705285/accepted-libsodium-1018-1deb11u1-source-into-oldoldstable-security/) for bullseye. This has been released as [**DLA 4435-1**](https://www.debian.org/lts/security/2025/DLA-4435-1).
  - **[ELTS]**: Fixed [CVE-2025-69277](https://security-tracker.debian.org/tracker/CVE-2025-69277) via **1.0.17-1+deb10u1** for buster. This has been released as [**ELA 1631-1**](https://www.freexian.com/lts/extended/updates/ela-1631-1-libsodium/).

- **ceph**: Improper validation of HTTP_X_AMZ_COPY_SOURCE header.
  - **[LTS]**: Fixed [CVE-2024-47866](https://security-tracker.debian.org/tracker/CVE-2024-47866) and [CVE-2022-0670](https://security-tracker.debian.org/tracker/CVE-2022-0670) via [**14.2.21-1+deb11u2**](https://tracker.debian.org/news/1711939/accepted-ceph-14221-1deb11u2-source-into-oldoldstable-security/) for bullseye. This has been released as [**DLA 4460-1**](https://www.debian.org/lts/security/2025/DLA-4460-1).
  - **[ELTS]**: Fixed [CVE-2024-47866](https://security-tracker.debian.org/tracker/CVE-2024-47866) via **12.2.11+dfsg1-2.1+deb10u3** for buster and **10.2.11-2+deb9u4** for stretch. This has been released as [**ELA 1632-1**](https://www.freexian.com/lts/extended/updates/ela-1632-1-ceph/).

- **modsecurity-apache**: Invalid request handling vulnerability.
  - **[ELTS]**: Fixed [CVE-2025-54571](https://security-tracker.debian.org/tracker/CVE-2025-54571) via **2.9.1-2+deb9u5** for stretch. This has been released as [**ELA 1633-1**](https://www.freexian.com/lts/extended/updates/ela-1633-1-modsecurity-apache/).

- **pyasn1**: Improper continuation octet limits in OID decoder.
  - **[LTS]**: Fixed [CVE-2026-23490](https://security-tracker.debian.org/tracker/CVE-2026-23490) via [**0.4.8-1+deb11u1**](https://tracker.debian.org/news/1712135/accepted-pyasn1-048-1deb11u1-source-into-oldoldstable-security/) for bullseye. This has been released as [**DLA 4463-1**](https://www.debian.org/lts/security/2025/DLA-4463-1).
  - **[ELTS]**: Fixed [CVE-2026-23490](https://security-tracker.debian.org/tracker/CVE-2026-23490) via **0.4.2-3+deb10u1** for buster and **0.1.9-2+deb9u1** for stretch. This has been released as [**ELA 1634-1**](https://www.freexian.com/lts/extended/updates/ela-1634-1-pyasn1/).

- **node-lodash**: Prototype pollution in baseUnset function.
  - **[unstable]**: Fixed [CVE-2025-13465](https://security-tracker.debian.org/tracker/CVE-2025-13465) via [**4.17.21+dfsg+~cs8.31.198.20210220-10**](https://tracker.debian.org/news/1712164/accepted-node-lodash-41721dfsgcs83119820210220-10-source-into-unstable/). This has been uploaded to unstable. DLA to follow once this has settled in sid and stable releases.

### Work in Progress

- **knot-resolver**: Affected by CVE-2023-26249, CVE-2023-46317, and CVE-2022-40188, leading to Denial of Service.
  - **[LTS]**: Some back and forth discussion with maintainers on the best way to proceed for the bullseye upload.
    - Git repository for bullseye: https://salsa.debian.org/lts-team/packages/knot-resolver/-/tree/debian/bullseye.

- **ruby-rack**: There were multiple vulnerabilities reported in Rack, leading to DoS (memory exhaustion) and proxy bypass.
  - **[ELTS]**: After completing the work for LTS myself, Bastien picked it up for ELTS and reached out about an upstream regression and we've been doing some exchanges. Bastien has done most of the work backporting the patches but needs a review and help backporting CVE-2025-61771. Haven't made much progress since last month and will carry it over.

- **node-lodash**: Affected by CVE-2025-13465, lrototype pollution in baseUnset function.
  - **[stable]**: The patch for trixie and bookworm are ready but haven't been uploaded yet as I'd like for the unstable upload to settle a bit before I proceed with stable uploads.
  - **[LTS]**: The bullseye upload will follow once the stable uploads are in and ACK'd by the SRMs.

- **xrdp**: Affected by CVE-2025-68670, leading to a stack-based buffer overflow.
  - **[LTS]**: Start to prep the work for bullseye and uploaded to Debusine: https://debusine.debian.net/debian/developers/work-request/367666. ELTS to follow.

### Other Activities

- **[ELTS]** Helped Bastien Roucaries debug a tomcat9 regression for buster.
  - I spent quite a lot of time trying to help Bastien (with Markus and Santiago involved via mail thread) by reproducing the regression that the user(s) reported.
  - I also helped suggest a path forward by vendoring everything, which I was then requested to also help perform.
  - Whilst doing that, I noticed circular dependency hellhole and suggested another path forward by backporting bnd and its dependencies as separate NEW packages.
  - Bastien liked the idea and is going to work on that but preferred to revert the update to remedy the immediate regressions reported. I further helped him in reviewing his update. This conversation happened on #debian-elts IRC channel.

- **[LTS]** Assisted Ben Hutchings with his question about the next possible steps with a plausible libvirt regression caused by the Linux kernel update. This was [a thread](https://lists.debian.org/debian-lts/2026/01/msg00011.html) on debian-lts@ mailing list.

- **[LTS]** Attended the monthly LTS meeting on IRC. [Summary here](https://meetbot.debian.net/debian-lts/2026/debian-lts.2026-01-22-14.00.html).

- **[E/LTS]** Monitored discussions on mailing lists, IRC, and all the documentation updates.

---

Until next time.  
`:wq` for today.
