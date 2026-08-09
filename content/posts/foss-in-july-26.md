+++
date = "2026-07-30 11:11:11 +0530"
title = "FOSS Activities in July 2026"
slug = "foss-in-july-26"
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

- Try to keep up with the threads around AI usage. :)
- Uploaded [node-lodash/4.17.21+dfsg+~cs8.31.198.20210220-9+deb13u1](https://tracker.debian.org/news/1778463/accepted-node-lodash-41721dfsgcs83119820210220-9deb13u1-source-into-proposed-updates/) to trixie to fix a couple of CVEs.
- Attended the Bursary BoF, remotely, in DebConf 26.

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

I joined [Canonical to work on Ubuntu full-time](https://utkarsh2102.org/posts/hello-canonical/) back in February 2021.

- Continued to push for infrastructure improvements:
  - Charming.
  - Artifact signing.
  - Reorganizing cdimage.
  - And so on.
- Assisted a bunch of folks with my Archive Admin and Release team hats to:
  - Promoting/demoting binaries to/from main.
  - Taking care of package removals and so on.
  - Reviewed the NEW queue.
- Reviewed quite a lot of MPs, specs, and other people's work.
- Mentoring, coaching, and leading the Release Management team.
- Mid-year break started and it was quite quiet for the last two weeks. I'll be off the first two weeks in August.

---

## Debian (E)LTS
{{< figure src="/images/debian-lts-small.png" >}}

This month I have worked 48.75 hours
on [Debian Long Term Support (LTS)](https://www.freexian.com/lts/debian/)
and on its sister [Extended LTS](https://www.freexian.com/lts/extended/)
project and did the following things:

### Released Security Updates

- **sympa**: Authentication bypass via an arbitrary e-mail address when the generic SSO login feature is enabled.
  - **[LTS]**: Fixed [CVE-2024-55919](https://security-tracker.debian.org/tracker/CVE-2024-55919) via [**6.2.70~dfsg-2+deb12u1**](https://tracker.debian.org/news/1771271/accepted-sympa-6270dfsg-2deb12u1-source-into-oldstable-security/) for bookworm. This has been released as [**DLA 4668-1**](https://www.debian.org/lts/security/2026/DLA-4668-1).

- **php8.2**: Buffer overflow in the AES Key Wrap with Padding implementation in the openssl extension, leading to memory corruption.
  - **[LTS]**: Fixed [CVE-2026-14355](https://security-tracker.debian.org/tracker/CVE-2026-14355) via [**8.2.32-1~deb12u1**](https://tracker.debian.org/news/1771272/accepted-php82-8232-1deb12u1-source-into-oldstable-security/) for bookworm. This has been released as [**DLA 4669-1**](https://www.debian.org/lts/security/2026/DLA-4669-1). Whilst at it, I also checked php7.4 in bullseye and marked it not-affected.

- **php-phpseclib**: Multiple vulnerabilities - a hostname validation bypass via subjectAltName, two timing side channels, an "OID amplification" denial of service in the ASN.1 decoder, and SSRF via the Authority Information Access extension.
  - **[LTS]**: Fixed [CVE-2023-52892](https://security-tracker.debian.org/tracker/CVE-2023-52892), [CVE-2026-32935](https://security-tracker.debian.org/tracker/CVE-2026-32935), [CVE-2026-40194](https://security-tracker.debian.org/tracker/CVE-2026-40194), [CVE-2026-44167](https://security-tracker.debian.org/tracker/CVE-2026-44167), and [CVE-2026-55599](https://security-tracker.debian.org/tracker/CVE-2026-55599) via [**2.0.30-2+deb11u3**](https://tracker.debian.org/news/1771254/accepted-php-phpseclib-2030-2deb11u3-source-into-oldoldstable-security/) for bullseye. This has been released as [**DLA 4670-1**](https://www.debian.org/lts/security/2026/DLA-4670-1). This is the one I'd carried over from last month; three more CVEs opened up in the meantime, so the final upload covers five instead of two.
  - **[ELTS]**: Fixed the same five CVEs via **2.0.30-2~deb10u4** for buster. This has been released as [**ELA 1785-1**](https://www.freexian.com/lts/extended/updates/ela-1785-1-php-phpseclib/).

- **wolfssl**: Multiple vulnerabilities, including X.509 name-constraint and CRL critical-extension bypasses, PKCS#7 signer confusion and MAC forgeries, and several memory-safety issues.
  - **[LTS]**: Fixed [CVE-2026-5194](https://security-tracker.debian.org/tracker/CVE-2026-5194), [CVE-2026-6092](https://security-tracker.debian.org/tracker/CVE-2026-6092), [CVE-2026-6094](https://security-tracker.debian.org/tracker/CVE-2026-6094), [CVE-2026-6325](https://security-tracker.debian.org/tracker/CVE-2026-6325), [CVE-2026-6329](https://security-tracker.debian.org/tracker/CVE-2026-6329), [CVE-2026-6331](https://security-tracker.debian.org/tracker/CVE-2026-6331), [CVE-2026-6450](https://security-tracker.debian.org/tracker/CVE-2026-6450), [CVE-2026-6678](https://security-tracker.debian.org/tracker/CVE-2026-6678), [CVE-2026-6681](https://security-tracker.debian.org/tracker/CVE-2026-6681), [CVE-2026-6731](https://security-tracker.debian.org/tracker/CVE-2026-6731), [CVE-2026-7511](https://security-tracker.debian.org/tracker/CVE-2026-7511), [CVE-2026-55961](https://security-tracker.debian.org/tracker/CVE-2026-55961), [CVE-2026-55962](https://security-tracker.debian.org/tracker/CVE-2026-55962), and [CVE-2026-55967](https://security-tracker.debian.org/tracker/CVE-2026-55967) via [**5.5.4-2+deb12u3**](https://tracker.debian.org/news/1774628/accepted-wolfssl-554-2deb12u3-source-into-oldstable-security/) for bookworm. This has been released as [**DLA 4683-1**](https://www.debian.org/lts/security/2026/DLA-4683-1).
  - This one had a bit of a story to it. I'd marked wolfssl end-of-life in bookworm earlier in the month (24 CVEs in one go), and then upstream turned up on the list offering patches for the 5.5.4 branch. So we un-EOL'd the subset upstream had covered, shipped them, and left the rest as-is. More on that below.

- **opam**: `.install` file directives were insufficiently restricted; symlink resolution on the target path wasn't checked, allowing directory traversal out of the package area.
  - **[LTS]**: Fixed [CVE-2026-57825](https://security-tracker.debian.org/tracker/CVE-2026-57825) via [**2.1.2-1+deb12u2**](https://tracker.debian.org/news/1774627/accepted-opam-212-1deb12u2-source-into-oldstable-security/) for bookworm. This has been released as [**DLA 4684-1**](https://www.debian.org/lts/security/2026/DLA-4684-1). The update itself was prepared by the OCaml team in their [Salsa repository](https://salsa.debian.org/ocaml-team/opam/-/tree/debian/bookworm); Salvatore reached out about this, so I claimed it and got it over the line.

- **squid**: Multiple vulnerabilities, which could result in information disclosure or Denial of Service.
  - **[LTS]**: Fixed [CVE-2026-33515](https://security-tracker.debian.org/tracker/CVE-2026-33515), [CVE-2026-33526](https://security-tracker.debian.org/tracker/CVE-2026-33526), [CVE-2026-47729](https://security-tracker.debian.org/tracker/CVE-2026-47729), and [CVE-2026-50012](https://security-tracker.debian.org/tracker/CVE-2026-50012) via [**4.13-10+deb11u7**](https://tracker.debian.org/news/1778027/accepted-squid-413-10deb11u7-source-into-oldoldstable-security/) for bullseye and [**5.7-2+deb12u6**](https://tracker.debian.org/news/1778028/accepted-squid-57-2deb12u6-source-into-oldstable-security/) for bookworm. This has been released as [**DLA 4697-1**](https://www.debian.org/lts/security/2026/DLA-4697-1).
  - **[ELTS]**: Fixed the same four CVEs via **4.13-10+deb11u7~deb10u1** for buster. This has been released as [**ELA 1782-1**](https://www.freexian.com/lts/extended/updates/ela-1782-1-squid/).
  - This was the big one for the month. Three suites, and CVE-2026-50012 needed a follow-up commit on top of the one upstream had flagged, which I noted in the tracker so the next person doesn't have to rediscover it.

### Work in Progress

- **phpseclib**: The 1.0.x source package, which is a separate source from php-phpseclib above.
  - **[LTS]**: 3 CVEs - [CVE-2026-44167](https://security-tracker.debian.org/tracker/CVE-2026-44167), [CVE-2026-40194](https://security-tracker.debian.org/tracker/CVE-2026-40194), and [CVE-2026-55599](https://security-tracker.debian.org/tracker/CVE-2026-55599) - are backported but haven't had the time to test the updates. This got pushed behind squid, so it'll be late Aug or early Sept's work.

- **node-lodash**: Following up on [DLA 4663-1](https://www.debian.org/lts/security/2026/DLA-4663-1).
  - **[LTS]**: We found a non-functional regression in the bullseye upload right at the start of the month and re-uploaded the fix to [debusine](https://debusine.debian.net/debian/developers/work-request/904322/) and was released upon successful testing.
  - **[bookworm]**: There's yet another regression there but this time, it's on upstream. I opened https://github.com/lodash/lodash/security/advisories/GHSA-fppw-337r-45gv to discuss this with upstream and so this will carry-over unfortunately.

### Other Activities

- **[E/LTS]** Did two front-desk weeks this month, 06-07 to 12-07 and 20-07 to 26-07. The second one wasn't originally mine - I swapped slots with Thorsten as I was leaving for vacation during the last weekend of July - and it turned out to be the busiest stretch of the month.
  - Across the two weeks I made **391 commits** to the LTS and ELTS security trackers - 381 hand-authored plus 10 automated ELTS end-of-life sweeps - triaging **505 unique CVEs** across **205 source packages** and all four suites.
  - Newly queued **28 source packages** - 26 in `dla-needed` (aom, chromium, clamav, exim4, ffmpeg, gimp, jackson-databind, libass, libde265, libxfont, logback, lrzip, opam, openimageio, py7zr, python-authlib, python-geopandas, python-git, python-httplib2, python-msgpack, redis, roundcube, ruby-oj, shiro, swift, and tiff) and 12 in `ela-needed` (clamav, gimp, gsasl, libass, libde265, libxfont, python-httplib2, python-msgpack, python-tornado, redis, ruby-oj, and tiff), 10 of them in both. Also widened 12 existing entries from a single suite to the whole tier - bind9, busybox, calibre, docker-registry, ffmpeg, ldap-account-manager, libcryptx-perl, libsoup2.4, python-tornado, and snapd on the LTS side, exim4 and ffmpeg on the ELTS one.
  - Most of the interesting work sat in the `<not-affected>` verdicts: **213 of 269** (79%, across 65 packages) rest on proving the vulnerable construct simply isn't in the source we ship, rather than on trusting upstream's affected-version range. Another 24 lines came from bundled or embedded libraries being out of scope - node-ajv uses uri-js and not the vulnerable fast-uri, jansi1 ships no native code, ruby-oj's flaw is JRuby-only, mina/mina2 don't ship the vulnerable sshd modules - and 10 from build configuration, e.g. curl is built `--without-libssh`, and there's no `libopenjp2-7-dev` in pillow's Build-Depends before bookworm, so the affected decoder isn't compiled in at all.
  - On the other side, 75 `<end-of-life>` lines, 72 of them in bookworm - lxd (28 CVEs), mbedtls (16), php-horde-imp, and php-horde-vfs - plus python2.7 in bullseye and golang-x-text in stretch. And some tracker hygiene: merged a stale RUSTSEC placeholder into the rust-quinn-proto entry, answered a long-standing hdf5 TODO about the array datatype decode, and flagged six entries where I reckon the Security team's trixie triage is off (rtklib, node-axios, openimageio, docker-registry, python3.9/python3.11, and the plainly wrong CNA text on CVE-2026-15308) to raise as one batch rather than acting on them unilaterally.
  - I even helped the Debian Security team in correcting a couple of their triages. We had exchanges over the mail.

- **[LTS]** Followed up on the wolfssl end-of-life question on the mailing list. Upstream offered to keep patching the 5.5.4 branch for bookworm, and my position was that end-of-life status and occasional opportunistic fixes can happily coexist - we should let it run over a few updates before considering flipping wolfssl back to limited-support, so we don't reverse an EOL decision we can't actually stand behind. [Thread here](https://lists.debian.org/debian-lts/2026/07/msg00036.html).

- **[LTS]** Reviewed Christopher's flask work for [CVE-2026-27205](https://security-tracker.debian.org/tracker/CVE-2026-27205) and flagged flask-socketio as a fresh regression in the reverse-dependency results before the upload went out. [Thread here](https://lists.debian.org/debian-lts/2026/07/msg00031.html).

- **[E/LTS]** Wrapped up my end of the security tracker repository size investigation from last month - ran the benchmarks on my own machine to satisfy myself the numbers held up, and then happily deferred to Sylvain, Helmut, and Santiago, who'd already put a lot more time into it and documented the workarounds. [Thread here](https://lists.debian.org/debian-lts/2026/07/msg00013.html).

- **[E/LTS]** Monitored discussions on mailing lists, IRC, and all the documentation updates.

- **[E/LTS]** Attended the monthly LTS meeting on IRC. [Meeting notes here](https://lists.debian.org/debian-lts/2026/07/msg00068.html).

---

Until next time.  
`:wq` for today.
