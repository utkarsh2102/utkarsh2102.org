+++
date = "2026-10-05 11:11:11 +0530"
title = "FOSS Activities in September 2026"
slug = "foss-in-sept-26"
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

Whilst I didn't have much time, here are still a few things that I worked on:

- Sponsored [ubuntu-dev-tools/0.214](https://tracker.debian.org/news/1798457/accepted-ubuntu-dev-tools-0214-source-into-unstable/) for Florent 'Skia' Jacquet, which updates `seeded-in-ubuntu` to use the new per-series indexer ([LP: #2160240](https://bugs.launchpad.net/bugs/2160240)).
- Assisted a few folks in getting their patches submitted via Salsa.
- Mentoring for newcomers.
- Moderation of -project mailing list.

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

I joined [Canonical to work on Ubuntu full-time](https://utkarsh2102.org/posts/hello-canonical/) back in February 2021.

- With 26.10 in Feature Freeze, wore my Release team hat to:
  - Review and approve a bunch of Feature Freeze Exceptions, including the Go 1.27 transition, Qt 6.11.2, rust-coreutils 0.12.0, devscripts 2.6.12, kdump-tools moving to dracut, and a few GCE packages.
  - Point linux-entra-sso to the SRU team, as it didn't need an FFe at all, and milestone a couple of bugs for 26.10.
- Continued to push for infrastructure improvements:
  - Made ubuntu-cdimage more resilient to Launchpad hiccups ([MP](https://code.launchpad.net/~utkarsh/ubuntu-cdimage/+git/ubuntu-cdimage/+merge/511948)).
  - Taught `generate-freeze-block` in ubuntu-archive-tools a couple of new options (`--skip-update` and `--series`) and better error handling ([MP](https://code.launchpad.net/~utkarsh/ubuntu-archive-tools/+git/ubuntu-archive-tools/+merge/511844)).
  - Bumped the arm64 generic non-cloud image to 4.5G in livecd-rootfs and uploaded it as [26.10.16](https://launchpad.net/ubuntu/+source/livecd-rootfs/26.10.16); also sponsored the follow-up [26.10.17](https://launchpad.net/ubuntu/+source/livecd-rootfs/26.10.17) for Chloé.
- Sponsored [aevol/9.4.0-2ubuntu1](https://launchpad.net/ubuntu/+source/aevol/9.4.0-2ubuntu1) for Matthieu, fixing an FTBFS with GCC 15's LTO ([LP: #2167811](https://bugs.launchpad.net/bugs/2167811)).
- Reviewed quite a lot of MPs - britney hints, meta-release, ubuntu-release-tools, ubuntu-archive-tools, ubuntu-cdimage, livecd-rootfs, ubuntu-seeds, and so on.
- Enabled [upgrades to 26.04 LTS](https://discourse.ubuntu.com/t/upgrades-from-ubuntu-24-04-lts-to-ubuntu-26-04-1-lts-now-enabled/88502).
- Released 26.10 Beta and [announced it on Discourse](https://discourse.ubuntu.com/t/ubuntu-26-10-stonking-stingray-beta-released/88662).
- Did Archive Admin, DMB, and Release team duties as usual.

---

## Debian (E)LTS
{{< figure src="/images/debian-lts-small.png" >}}

This month I have worked 33.5 hours
on [Debian Long Term Support (LTS)](https://www.freexian.com/lts/debian/)
and on its sister [Extended LTS](https://www.freexian.com/lts/extended/)
project and did the following things:

(A quick note that I did quite a lot of the work during my work as Frontdesk that went on till 4th Oct, so 33.50 hours include the work I did till 4th October 2026.)

### Released Security Updates

- **node-lodash**: Prototype pollution in `_.unset` and `_.omit` (plus a bypass of the initial fix for it), and code injection via the `imports` option of `_.template`.
  - **[LTS]**: Fixed [CVE-2025-13465](https://security-tracker.debian.org/tracker/CVE-2025-13465), [CVE-2026-2950](https://security-tracker.debian.org/tracker/CVE-2026-2950), and [CVE-2026-4800](https://security-tracker.debian.org/tracker/CVE-2026-4800) via [**4.17.21+dfsg+~cs8.31.198.20210220-9+deb12u1**](https://tracker.debian.org/news/1806836/accepted-node-lodash-41721dfsgcs83119820210220-9deb12u1-source-into-oldstable-security/) for bookworm. This has been released as [**DLA 4820-1**](https://www.debian.org/lts/security/2026/DLA-4820-1).
  - This is the bookworm follow-up to DLA 4663-1 that I carried over from July. The update had been sitting prepared and tested on [debusine](https://debusine.debian.net/debian/developers/work-request/908246/), so once the upstream discussion wrapped up, it went straight out. It also carries an extra patch to the lodash-cli dependency map - without it, the regenerated `lodash.template` module throws "assignWith is not defined" at runtime, which node-gulp-util's autopkgtest caught.

- **libpng1.6**: Use-after-free of zlib input in `png_read_end()` after incomplete zTXt, iTXt, or iCCP decompression, which could result in denial of service.
  - **[LTS]**: Fixed [CVE-2026-46675](https://security-tracker.debian.org/tracker/CVE-2026-46675) via [**1.6.39-2+deb12u6**](https://tracker.debian.org/news/1807401/accepted-libpng16-1639-2deb12u6-source-into-oldstable-security/) for bookworm. This has been released as [**DLA 4824-1**](https://www.debian.org/lts/security/2026/DLA-4824-1).
  - I picked this one up whilst on front desk; the upstream fix that went into trixie via [DSA 6537-1](https://lists.debian.org/debian-security-announce/2026/msg00450.html) applied to 1.6.39 as-is.

### Work in Progress

- **libpng1.6**: The same CVE-2026-46675.
  - **[ELTS]**: Claimed in `ela-needed`; the same upstream fix applies to all three ELTS suites, so this should go out shortly.

### Other Activities

- **[E/LTS]** Did my front-desk week from 28-09 to 04-10.
  - Over the week I made **369 commits** to the LTS and ELTS security trackers - 368 hand-authored plus 1 automated ELTS end-of-life sweep.
    - The hand-authored ones cover **524 unique CVEs** across **192 source packages** and all four suites.
    - Additional data is now part of the front-desk job too, so 75 of those commits record it for 179 CVEs across 71 packages.
  - Newly queued **22 source packages** - 13 in `dla-needed` (apache2, chromium, firefox-esr, libnet-idn-encode-perl, libpng1.6, node-shell-quote, nvidia-graphics-drivers, openssl, pcre2, php-mongodb, php8.2, social-auth-core, and wpa) and 16 in `ela-needed` (apache2, firefox-esr, gegl, lemonldap-ng, libnet-idn-encode-perl, libpng1.6, libwebsockets, nsd, nvidia-graphics-drivers, pcre2, php7.0, php7.3, php7.4, rar, unrar-nonfree, and wpa), 7 of them in both. Also widened 3 ELTS entries to bullseye - antiword, ocaml, and openvswitch.
  - Most of the interesting work was again in the `<not-affected>` verdicts: **217 of 263** (83%, across 57 packages) rest on showing that the vulnerable code or feature isn't in the source we ship. Another 17 cover incomplete upstream fixes that we either never shipped or shipped with the follow-up already in (expat, libxml2, node-tar, and pyjwt). 15 come from bundled components we don't ship - node-ajv again, which uses uri-js and not fast-uri, and nvidia-open, which doesn't ship the NGX updater. And 13 are vendor- or platform-specific - openssh's CVE-2026-55654 lives only in a Red Hat GSSAPI patch, and the netdata and PHP ones only affect Windows.
  - Did 4 rounds of newly supported bullseye packages (33 packages overall), plus libmail-mboxparser-perl for buster - 34 in all. The existing CVE data mostly held up; the real finds were discovery gaps. One interesting gotcha: sid renamed stunnel4 to stunnel, and two new CVEs were associated only with the new name, so they never showed up for trixie, bookworm, or any ELTS suite. I also sorted the 180 "Triage needed" entries (57 packages) from elts-eol by where each was already handled, and triaged for ELTS the 100 that trixie or bookworm had already decided; the rest come next. And I imported 79 package-level lines for the older source names ELTS still ships (tomcat8, php7.0/7.3/7.4, netty-3.9, openssl1.0, python2.7/3.5/3.7, and pypy).
  - Caught some inconsistencies in released advisories: DLA 4801-1 (swift) was missing a CVE, ELA 1831-1 (redis) listed the wrong one, and DLA 4808-1 (network-manager-l2tp) listed CVE-2026-75883 - an ID that was renamed and then reassigned to an unrelated ppp issue. I fixed all three in the tracker's advisory lists.
  - Made the Security team and the uploaders aware of regressions from our own updates:
    - libde265: the CVE-2026-49337 fix in DLA 4789-1/ELA 1828-1 (and DSA 6413-1) misses upstream's follow-up commit.
    - libxml2 CVE-2026-76781 and policykit-1 CVE-2026-85498 were introduced by our own back-ports; the policykit-1 one is harmless.
    - expat: the CVE-2025-59375 backport in DLA 4807-1 is compiled out, because `XML_GE` is never defined.
    - xen: DLA 4818-1's XSA-491 fix makes XSA-510 reachable.
    - gegl: the CVE-2026-2049/2050 back-port in ELA 1650-1 rejects valid RLE .hdr files.
    - log4cxx: DLA 4322-1 broke UTF-8 in JSONLayout output. That one is functional, not security.
  - Helped correct a set of triages and let the Debian Security team know:
    - ruby-json CVE-2026-71847: the vulnerable code was never in a released Debian version.
    - openssh CVE-2026-55654: only affects a Red Hat-specific GSSAPI patch.
    - three libxml2 issues that don't affect trixie either.
    - the stunnel4 rename above.
    - trixie `<no-dsa>` lines on jsch, node-qs, and ruby-loofah, where trixie's version doesn't have the vulnerable feature at all.
  - Independently found a security issue in rclone and reported it privately upstream through a GitHub security advisory. Upstream already had a report for the same issue, so they folded mine into the existing advisory and credited me as a co-reporter. More once it's public.
    - https://github.com/rclone/rclone/security/advisories/GHSA-66qv-66mg-9h74
  - Also found some bugs in the additional-data tooling, e.g. `cve-ad --package P --severity tbd` wipes the CVE-level severity, and the schema doesn't validate package-level entries at all.

- **[E/LTS]** Monitored discussions on mailing lists, IRC, and all the documentation updates.

- **[E/LTS]** Attended the monthly LTS meeting on IRC. [Meeting notes here](https://lists.debian.org/debian-lts/2026/09/msg00091.html).

---

Until next time.  
`:wq` for today.
