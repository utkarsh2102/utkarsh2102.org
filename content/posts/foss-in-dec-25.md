+++
date = "2025-12-30 11:11:11 +0530"
title = "FOSS Activites in December 2025"
slug = "foss-in-dec-25"
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

- Prepared security update for wordpress for trixie and bookworm.
- A few discussions with the new DFSG team, et al.
- Assited a few folks in getting their patches submitted via Salsa.
- Mentoring for newcomers.
- Moderation of -project mailing list.

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

I joined [Canonical to work on Ubuntu full-time](https://utkarsh2102.org/posts/hello-canonical/) back in February 2021.

Whilst I can't give a full, detailed list of things I did, here's a quick TL;DR of what I did:

- Successfully released [Resolute Snapshot 2](https://discourse.ubuntu.com/t/resolute-snapshot-2-released/73478)!
  - This one was also done without the ISO tracker and cdimage access.
  - I think this one went rather smooth. Let's see what we're able to do for snapshot 3.
- Worked on removing GPG keys from the cdimage instance. That took a while, whew!
- Assisted a bunch of folks with my Archive Admin and Release team hats to:
  - review NEW packages for Ubuntu Studio.
  - remove old binaries that are stalling transition and/or migration.
  - LTS requalification of Ubuntu flavours.
  - bootstrapping dotnet-10 packages for Stable Release Updates.
- With that, we've entered the EOY break. :)
  - I was anyway on vacation for majority of this month. ;)

---

## Debian (E)LTS
{{< figure src="/images/debian-lts-small.png" >}}

This month I have worked 72 hours
on [Debian Long Term Support (LTS)](https://www.freexian.com/lts/debian/)
and on its sister [Extended LTS](https://www.freexian.com/lts/extended/)
project and did the following things:

### Released Security Updates

- **ruby-git**: Multiple vulnerabilities leading to command line injection and improper path escaping.
  - **[LTS]**: Fixed [CVE-2022-25648](https://security-tracker.debian.org/tracker/CVE-2022-25648), [CVE-2022-46648](https://security-tracker.debian.org/tracker/CVE-2022-46648), and [CVE-2022-47318](https://security-tracker.debian.org/tracker/CVE-2022-47318) via [**1.7.0-1+deb11u1**](https://tracker.debian.org/news/1698358/accepted-ruby-git-170-1deb11u1-source-into-oldoldstable-security/) for bullseye. This has been released as [**DLA 4406-1**](https://www.debian.org/lts/security/2025/DLA-4406-1).

- **ruby-sidekiq**: Multiple vulnerabilities leading to Cross-site Scripting (XSS) and Denial of Service in Web UI.
  - **[LTS]**: Fixed [CVE-2021-30151](https://security-tracker.debian.org/tracker/CVE-2021-30151) and [CVE-2022-23837](https://security-tracker.debian.org/tracker/CVE-2022-23837) via [**6.0.4+dfsg-2+deb11u1**](https://tracker.debian.org/news/1698365/accepted-ruby-sidekiq-604dfsg-2deb11u1-source-into-oldoldstable-security/) for bullseye. This has been released as [**DLA 4407-1**](https://www.debian.org/lts/security/2025/DLA-4407-1).

- **python-apt**: Vulnerability leading to crash via invalid nullptr dereference in TagSection.keys().
  - **[LTS]**: Fixed [CVE-2025-6966](https://security-tracker.debian.org/tracker/CVE-2025-6966) via [**2.2.1.1**](https://tracker.debian.org/news/1698383/accepted-python-apt-2211-source-into-oldoldstable-security/) for bullseye. This has been released as [**DLA 4408-1**](https://www.debian.org/lts/security/2025/DLA-4408-1).
  - **[ELTS]**: Fixed [CVE-2025-6966](https://security-tracker.debian.org/tracker/CVE-2025-6966) via **1.8.4.4** for buster and **1.4.4** for stretch. This has been released as [**ELA 1596-1**](https://www.freexian.com/lts/extended/updates/ela-1596-1-python-apt/).
  - All of this was coordinated b/w the Security team and Julian Andres Klode. Julian will take care of the stable uploads.

- **node-url-parse**: Vulnerability allowing authorization bypass through specially crafted URL with empty userinfo and no host.
  - **[LTS]**: Fixed [CVE-2022-0639](https://security-tracker.debian.org/tracker/CVE-2022-0639) via [**1.5.3-1+deb11u3**](https://tracker.debian.org/news/1698861/accepted-node-url-parse-153-1deb11u3-source-into-oldoldstable-security/) for bullseye. This has been released as [**DLA 4413-1**](https://www.debian.org/lts/security/2025/DLA-4413-1).

- **wordpress**:  Multiple vulnerabilities in WordPress core, leading to Sent Data & Cross-site Scripting.
  - **[stable]**: Fixed [CVE-2025-58674](https://security-tracker.debian.org/tracker/CVE-2025-58674) and [CVE-2025-58246](https://security-tracker.debian.org/tracker/CVE-2025-58246) via [**6.8.3+dfsg1-0+deb13u1**](https://tracker.debian.org/news/1700127/accepted-wordpress-683dfsg1-0deb13u1-source-into-proposed-updates/) for trixie.  This has been released as [**DSA 6091-1**](https://www.debian.org/security/2025/dsa-6091).

- **usbmuxd**: Privilege escalation vulnerability via path traversal in SavePairRecord command.
  - **[LTS]**: Fixed [CVE-2025-66004](https://security-tracker.debian.org/tracker/CVE-2025-66004) via [**1.1.1-2+deb11u1**](https://tracker.debian.org/news/1699488/accepted-usbmuxd-111-2deb11u1-source-into-oldoldstable-security/) for bullseye. This has been released as [**DLA 4417-1**](https://www.debian.org/lts/security/2025/DLA-4417-1).
  - **[ELTS]**: Fixed [CVE-2025-66004](https://security-tracker.debian.org/tracker/CVE-2025-66004) via **1.1.1~git20181007.f838cf6-1+deb10u1** for buster and **1.1.0-2+deb9u1** for stretch. This has been released as [**ELA 1599-1**](https://www.freexian.com/lts/extended/updates/ela-1599-1-usbmuxd/).
  - All of this was coordinated b/w the Security team and Yves-Alexis Perez. Yves will take care of the stable uploads.

- **gst-plugins-good1.0**: Multiple vulnerabilities in isomp4 plugin leading to potential out-of-bounds reads and information disclosure.
  - **[LTS]**:  Fixed [CVE-2025-47219](https://security-tracker.debian.org/tracker/CVE-2025-47219) and [CVE-2025-47183](https://security-tracker.debian.org/tracker/CVE-2025-47183) via [**1.18.4-2+deb11u4**](https://tracker.debian.org/news/1701009/accepted-gst-plugins-good10-1184-2deb11u4-source-into-oldoldstable-security/) for bullseye. This has been released as [**DLA 4419-1**](https://www.debian.org/lts/security/2025/DLA-4419-1).

- **postgresql-13**: Multiple vulnerabilities including unauthorized schema statistics creation and integer overflow in libpq allocation calculations.
  - **[LTS]**:  Fixed [CVE-2025-12817](https://security-tracker.debian.org/tracker/CVE-2025-12817) and [CVE-2025-12818](https://security-tracker.debian.org/tracker/CVE-2025-12818) via [**13.23-0+deb11u1**](https://tracker.debian.org/news/1701263/accepted-postgresql-13-1323-0deb11u1-source-into-oldoldstable-security/) for bullseye. This update has been prepared by the maintainer, Christoph Berg, and released as [**DLA 4420-1**](https://www.debian.org/lts/security/2025/DLA-4420-1).

- **gst-plugins-base1.0**:  Multiple vulnerabilities in SubRip subtitle parsing leading to potential crashes and buffer issues.
  - **[ELTS]**: Fixed [CVE-2025-47806](https://security-tracker.debian.org/tracker/CVE-2025-47806), [CVE-2025-47807](https://security-tracker.debian.org/tracker/CVE-2025-47807), and [CVE-2025-47808](https://security-tracker.debian.org/tracker/CVE-2025-47808) via **1.14.4-2+deb10u5** for buster and **1.10.4-1+deb9u6** for stretch.  This has been released as [**ELA 1600-1**](https://www.freexian.com/lts/extended/updates/ela-1600-1-gst-plugins-base1.0/).


### Work in Progress

- **ceph**: Affected by CVE-2024-47866, using the argument `x-amz-copy-source` to put an object and specifying an empty string as its content leads to the RGW daemon crashing, resulting in a DoS attack.
  - **[LTS]**: Whilst the patch is straightforward, backports are a bit tricky. Also trying to backport the fix for CVE-2022-0670. The update has been prepared as of December 16th and awaiting Thomas Goirand's review.
    - Git repository for bullseye: https://salsa.debian.org/lts-team/packages/ceph/-/tree/debian/bullseye.
  - **[ELTS]**: Same as LTS - I've tested the update but waiting for Thomas to ack the LTS upload and so I can proceed with ELTS uploads.
    - Git repository for buster: http://salsa.debian.org/lts-team/packages/ceph/-/commits/debian/buster
    - Git repository for stretch: http://salsa.debian.org/lts-team/packages/ceph/-/commits/debian/stretch

- **knot-resolver**: Affected by CVE-2023-26249, CVE-2023-46317, and CVE-2022-40188, leading to Denial of Service.
  - **[LTS]**: The patches aren't very trivial, with
CVE-2023-46317 reverting much of the patch for CVE-2023-26249. And then it had to be re-adjusted a bit for v5.3.1. The backports are ready as of December 23rd and awaiting Jakub or Santiago's review.
    - Git repository for bullseye: https://salsa.debian.org/lts-team/packages/knot-resolver/-/tree/debian/bullseye

- **adminer**: Affected by CVE-2023-45195 and CVE-2023-45196, leading to SSRF and DoS, respectively.
  - **[ELTS]**: I picked it up again and the patches were already ready in Git. I've reached out to Alexandre for a quick review and smoke test before we can release it for buster.
    - Git repository for buster: https://salsa.debian.org/lts-team/packages/adminer/-/tree/debian/buster

- **u-boot**: Affected by CVE-2025-24857, where boot code access control flaw in U-Boot allowing arbitrary code execution via physical access.
  - **[ELTS]**: As it's only affected the version in stretch, I've started the work to find the fixing commits and prepare a backport. Not much progress there, I'll roll it over to January.

- **ruby-rack**: There were multiple vulnerabilities reported in Rack, leading to DoS (memory exhaustion) and proxy bypass.
  - **[ELTS]**: After completing the work for LTS myself, Bastien picked it up for ELTS and reached out about an upstream regression and we've been doing some exchanges. Bastien has done most of the work backporting the patches but needs a review and help backporting CVE-2025-61771.

### Other Activities

- Frontdesk from 01-12-2025 to 07-12-2025.
  - Auto EOL'd a bunch of packages.
  - Marked CVE-2025-12084/python2.7 as end-of-life for bullseye, buster, and stretch.
  - Marked CVE-2025-12084/jython as end-of-life for bullseye.
  - Marked CVE-2025-13992/chromium as end-of-life for bullseye.
  - Marked apache2 CVEs as postponed for bullseye, buster, and stretch.
  - Marked CVE-2025-13654/duc as postponed for bullseye and buster.
  - Marked CVE-2025-32900/kdeconnect as ignored for bullseye.
  - Marked CVE-2025-12084/pypy3 as postponed for bullseye.
  - Marked CVE-2025-14104/util-linux as postponed for bullseye, buster, and stretch.
  - Marked several CVEs for fastdds as postponed for bullseye.
  - Marked several CVEs for pytorch as postponed for bullseye.
  - Marked CVE-2025-2486/edk2 as postponed for bullseye.
  - Marked CVE-2025-6172{7,9}/golang-1.15 as postponed for bullseye.
  - Marked CVE-2025-65637/golang-logrus as postponed for bullseye.
  - Marked CVE-2025-12385/qtdeclarative-opensource-src{,gles} as postponed for bullseye, buster, and stretch.
  - Marked TEMP-0000000-D08402/rust-maxminddb as postponed for bullseye.
  - Added the following packages to {d,e}la-needed.txt:
    - liblivemedia, sogo.
  - During my triage, I had to make the bin/elts-eol script robust to determine the `lts_admin` repository - did a back and forth with Emilio about this on the list.
  - I sent a gentle reminder to the LTS team about the issues fixed in bullseye but not in bookworm via mailing list: https://lists.debian.org/debian-lts/2025/12/msg00013.html.


- I claimed php-horde-css-parser to work on CVE-2020-13756 for buster and did almost all the work only to realize that the patch already existed in buster and the changelog confirmed that it was intentionally fixed.
  - After speaking with Andreas Henriksson, we figured that the CVE ID was missed when the ELA was generated and so I fixed that via 87afaaf19ce56123bc9508d9c6cd5360b18114ef and 5621431e84818b4e650ffdce4c456daec0ee4d51 in the ELTS security tracker to reflect the situation.

- Participated in a thread which I started last month around using Salsa CI for E/LTS packages and if we plan to sunset it in favor of using Debusine. The plan for now is to keep it around as it's still beneficial and Debusine is still in its early phase.

- Did a lot of back and forth with Helmut about debusine uploads on #debian-elts.
  - While debugging a failure in dcut uploads, I ran into an SSH compatibility issue on deb-master.freexian.com that could be fixed on the server-side. I shared all my findings to Freexian's sysadmin team.
  - A minimal fix on the server side would be one of:
    ```
    PubkeyAcceptedAlgorithms -ssh-dss
    ```
    or explicitly restricting to modern algorithms, e.g.:
    ```
    PubkeyAcceptedAlgorithms
    ssh-ed25519,ecdsa-sha2-nistp256,rsa-sha2-512,rsa-sha2-256
    ```

- Jelly on #debian-lts reported that all my DLA mails had broken GMail's DKIM signature. So I set up sending replies from @debian.org and that seems to have fixed that! \o/

- **[LTS]** Attended a rather short monthly LTS meeting on Jitsi. [Summary here](https://lists.debian.org/debian-lts/2025/12/msg00032.html).

- **[E/LTS]** Monitored discussions on mailing lists, IRC, and all the documentation updates.

---

Until next time.  
`:wq` for today.
