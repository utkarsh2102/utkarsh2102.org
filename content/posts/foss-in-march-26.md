+++
date = "2026-03-30 11:11:11 +0530"
title = "FOSS Activites in March 2026"
slug = "foss-in-march-26"
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

- A quick exchange with Xavier about node-lodash fixes for stable releases.
- Uploaded ruby-rack to CVE-2026-25500 & CVE-2026-22860 to sid, trixie, and bookworm.
- Started to work on the DebConf Bursary team along with PEB.
- Assited a few folks in getting their patches submitted via Salsa.
- Mentoring for newcomers.
- Moderation of -project mailing list.

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

I joined [Canonical to work on Ubuntu full-time](https://utkarsh2102.org/posts/hello-canonical/) back in February 2021.

Whilst I can't give a full, detailed list of things I did, here's a quick TL;DR of what I did:

- Successfully released [26.04 LTS Beta](https://discourse.ubuntu.com/t/ubuntu-26-04-lts-resolute-raccoon-beta-released/79205)!
  - This one was also done without the ISO tracker and cdimage access.
  - We also worked very hard to build and promote all the image in due time.
  - This was the first proper milestone with the Test Observer.
  - We also did a retrospective: https://discourse.ubuntu.com/t/26-04-beta-tests-ubuntu-com-retrospective/79853.
- Worked further on the whole artifact signing story for cdimage.
- Assisted a bunch of folks with my Archive Admin and Release team hats to:
  - Review and grant FFes.
  - Coordinating weekly syncs.
  - Promoting/demoting binaries to/from main.
  - Taking care of package removals and so on.
- Was pretty occupied with the new release processs architecture and design.
- Preparing for the 26.04 LTS final release.

---

## Debian (E)LTS
{{< figure src="/images/debian-lts-small.png" >}}

This month I have worked 50 hours
on [Debian Long Term Support (LTS)](https://www.freexian.com/lts/debian/)
and on its sister [Extended LTS](https://www.freexian.com/lts/extended/)
project and did the following things:

### Released Security Updates

- **libvirt**: Regression introduced by the linux kernel update via DLA 4404-1.
  - **[LTS]**: Fixed the regression (Debian bug #1124549) via [**7.0.0-3+deb11u4**](https://tracker.debian.org/news/1732303/accepted-libvirt-700-3deb11u4-source-into-oldoldstable-security/) for bullseye. This has been released as [**DLA 4504-1**](https://www.debian.org/lts/security/2026/DLA-4504-1).

- **ruby-rack**: Path traversal and stored XSS vulnerabilities in directory handling.
  - **[LTS]**: Fixed [CVE-2026-22860](https://security-tracker.debian.org/tracker/CVE-2026-22860) and [CVE-2026-25500](https://security-tracker.debian.org/tracker/CVE-2026-25500) via [**2.1.4-3+deb11u5**](https://tracker.debian.org/news/1733701/accepted-ruby-rack-214-3deb11u5-source-into-oldoldstable-security/) for bullseye. This has been released as [**DLA 4505-1**](https://www.debian.org/lts/security/2026/DLA-4505-1).
  - **[bookworm]**: Fixed [CVE-2026-22860](https://security-tracker.debian.org/tracker/CVE-2026-22860) and [CVE-2026-25500](https://security-tracker.debian.org/tracker/CVE-2026-25500) via [**2.2.2-0+deb12u1**](https://tracker.debian.org/news/1735337/accepted-ruby-rack-2222-0deb12u1-source-into-oldstable-security/) for bookworm. This has been uploaded to oldstable-security.
  - **[trixie]**: Fixed [CVE-2026-22860](https://security-tracker.debian.org/tracker/CVE-2026-22860) and [CVE-2026-25500](https://security-tracker.debian.org/tracker/CVE-2026-25500) via [**3.1.2-0+deb13u1**](https://tracker.debian.org/news/1735338/accepted-ruby-rack-3120-0deb13u1-source-into-stable-security/) for trixie. This has been uploaded to stable-security.

- **vlc**: Out-of-bounds read and denial of service via a crafted MMS server response.
  - **[LTS]**: Fixed [CVE-2025-51602](https://security-tracker.debian.org/tracker/CVE-2025-51602) via [**3.0.23-0+deb11u1**](https://tracker.debian.org/news/1733900/accepted-vlc-3023-0deb11u1-source-into-oldoldstable-security/) for bullseye. This has been released as [**DLA 4507-1**](https://www.debian.org/lts/security/2026/DLA-4507-1).
  - **[ELTS]**: The 3.0.23 backport is ready but still in testing. Will be released in April.

- **nss**: Integer overflow in the AES-GCM implementation.
  - **[LTS]**: Fixed [CVE-2026-2781](https://security-tracker.debian.org/tracker/CVE-2026-2781) via [**2:3.61-1+deb11u5**](https://tracker.debian.org/news/1734200/accepted-nss-3611deb11u5-source-into-oldoldstable-security/) for bullseye. This has been released as [**DLA 4508-1**](https://www.debian.org/lts/security/2026/DLA-4508-1).

- **gst-plugins-base1.0**: Integer overflow in the RIFF parser.
  - **[LTS]**: Fixed [CVE-2026-2921](https://security-tracker.debian.org/tracker/CVE-2026-2921) via [**1.18.4-2+deb11u5**](https://tracker.debian.org/news/1734600/accepted-gst-plugins-base10-1184-2deb11u5-source-into-oldoldstable-security/) for bullseye. This has been released as [**DLA 4514-1**](https://www.debian.org/lts/security/2026/DLA-4514-1).
  - **[ELTS]**: Fixed [CVE-2026-2921](https://security-tracker.debian.org/tracker/CVE-2026-2921) via **1.14.4-2+deb10u6** for buster and **1.10.4-1+deb9u7** for stretch. This has been released as [**ELA 1669-1**](https://www.freexian.com/lts/extended/updates/ela-1669-1-gst-plugins-base1.0/).

- **gst-plugins-ugly1.0**: Heap-based buffer overflow and out-of-bounds write in media demuxers.
  - **[LTS]**: Fixed [CVE-2026-2920](https://security-tracker.debian.org/tracker/CVE-2026-2920) and [CVE-2026-2922](https://security-tracker.debian.org/tracker/CVE-2026-2922) via [**1.18.4-2+deb11u2**](https://tracker.debian.org/news/1734700/accepted-gst-plugins-ugly10-1184-2deb11u2-source-into-oldoldstable-security/) for bullseye. This has been released as [**DLA 4516-1**](https://www.debian.org/lts/security/2026/DLA-4516-1).
  - **[ELTS]**: Fixed [CVE-2026-2920](https://security-tracker.debian.org/tracker/CVE-2026-2920) and [CVE-2026-2922](https://security-tracker.debian.org/tracker/CVE-2026-2922) via **1.14.4-1+deb10u3** for buster and **1.10.4-1+deb9u3** for stretch. This has been released as [**ELA 1670-1**](https://www.freexian.com/lts/extended/updates/ela-1670-1-gst-plugins-ugly1.0/).

- **phpseclib**: Name confusion in X.509 certificate verification and a padding oracle timing attack in AES-CBC.
  - **[LTS]**: Fixed [CVE-2023-52892](https://security-tracker.debian.org/tracker/CVE-2023-52892) and [CVE-2026-32935](https://security-tracker.debian.org/tracker/CVE-2026-32935) via [**1.0.19-3+deb11u3**](https://tracker.debian.org/news/1734900/accepted-phpseclib-1019-3deb11u3-source-into-oldoldstable-security/) for bullseye. This has been released as [**DLA 4518-1**](https://www.debian.org/lts/security/2026/DLA-4518-1).
  - **[ELTS]**: Fixed [CVE-2023-52892](https://security-tracker.debian.org/tracker/CVE-2023-52892) and [CVE-2026-32935](https://security-tracker.debian.org/tracker/CVE-2026-32935) via **1.0.19-3~deb10u4** for buster. This has been released as [**ELA 1671-1**](https://www.freexian.com/lts/extended/updates/ela-1671-1-phpseclib/).

### Work in Progress

- **knot-resolver**: Affected by CVE-2023-26249, CVE-2023-46317, and CVE-2022-40188, leading to Denial of Service.
  - **[LTS]**: Still in back and forth discussion with maintainers on the best way to proceed for the bullseye upload. Git repository for bullseye: https://salsa.debian.org/lts-team/packages/knot-resolver/-/tree/debian/bullseye.

- **node-lodash**: Affected by [CVE-2025-13465](https://security-tracker.debian.org/tracker/CVE-2025-13465), prototype pollution in the `baseUnset` function.
  - **[stable]**: Xavier from the JS team ACK'd the patch. The trixie and bookworm uploads will follow.
  - **[LTS]**: The bullseye test and upload will follow in April once the stable uploads are in and ACK'd by the SRMs.

- **vlc**: Affected by CVE-2025-51602, an out-of-bounds read and denial of service via a crafted 0x01 response from an MMS server.
  - **[LTS]**: 3.0.23 backport is ready but not tested. I'll get this over the line in March.
  - **[ELTS]**: 3.0.23 backport is ready but not very clean. Would like to complete LTS and get back to this.


### Other Activities

- **[ELTS]** Continued to review ruby-rack for ELTS -- it has since received about 13 new CVEs, making it even more chaotic. Might consider releasing in batches.

- **[E/LTS]** Monitored discussions on mailing lists, IRC, and all the documentation updates.

- **[E/LTS]** Attended the monthly LTS meeting on IRC. [Summary here](https://meetbot.debian.net/debian-lts/2026/debian-lts.2026-03-26-14.00.html).

- **[Other]** Spent quite some time debugging a bug in debusine. Filed https://salsa.debian.org/freexian-team/debusine/-/issues/1412 for the same. Have worked on a preliminary patch but would like to submit something for Colin to review. Will follow up in April.

---

Until next time.  
`:wq` for today.
