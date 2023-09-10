+++
date = "2023-08-30 11:11:11 +0530"
title = "FOSS Activites in August 2023"
slug = "foss-in-aug-23"
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

Here's my (forty-seventh) monthly but brief update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 56th month of actively contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March 2019 and a [DD](https://wiki.debian.org/DebianDeveloper) on Christmas '19! \o/

There's a bunch of things I do, both, technical and non-technical. Here are the things I did this month:

### Uploads

- [pystaticconfiguration](https://tracker.debian.org/pkg/pystaticconfiguration) (0.11.1-1) - New upstream version, v0.11.1.
- [python-jira](https://tracker.debian.org/pkg/python-jira) (3.5.2-1) - New upstream version, v3.5.2.
- [django-modeltranslation](https://tracker.debian.org/pkg/django-modeltranslation) (0.18.11-1) - New upstream version, v0.18.11.
- [python-stomp](https://tracker.debian.org/pkg/python-stomp) (8.1.0-1) - New upstream version, v8.1.0.
- [python-twilio](https://tracker.debian.org/pkg/python-twilio) (8.6.0-1) - New upstream version, v8.6.0.

### Others

- Mentoring for newcomers.
- Bug work and debugging issues for ccextractor.
- Sponsored the upload of blueman for Christopher Schramm.
- DebConf Bursary work w/ bursary lead hat on.
- Helping DebConf orga w/ other things as DebConf is around the corner.
- Moderation of -project mailing list.

A huge thanks to Freexian for sponsoring my Debian work. :D

---

## Ubuntu
{{< figure src="/images/ubuntu-logo-small.png" >}}

This was my 31st month of actively contributing to [Ubuntu](https://ubuntu.com/about).
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

This was my forty-seventh month as a Debian LTS and thirty-fourth month as a Debian ELTS paid contributor.  
I worked for 12.25 hours for LTS and 72.50 hours for ELTS.

#### LTS Work:

- Issued [DLA 3529-1](https://lists.debian.org/debian-lts-announce/2023/08/msg00018.html), fixing [CVE-2021-23445](https://security-tracker.debian.org/tracker/CVE-2021-23445), for [datatables.js](https://tracker.debian.org/pkg/datatables.js).  
  For Debian 10 buster, these problems have been fixed in version 1.10.19+dfsg-1+deb10u1.
- Issued [DLA 3531-1](https://lists.debian.org/debian-lts-announce/2023/08/msg00020.html), fixing [CVE-2023-20867](https://security-tracker.debian.org/tracker/CVE-2023-20867), for [open-vm-tools](https://tracker.debian.org/pkg/open-vm-tools).  
  For Debian 10 buster, these problems have been fixed in version 2:10.3.10-1+deb10u4.
- Issued [DLA 3532-1](https://lists.debian.org/debian-lts-announce/2023/08/msg00021.html), fixing [CVE-2023-38408](https://security-tracker.debian.org/tracker/CVE-2023-38408), for [openssh](https://tracker.debian.org/pkg/openssh).  
  For Debian 10 buster, these problems have been fixed in version 1:7.9p1-10+deb10u3.
- Issued [DLA 3537-1](https://lists.debian.org/debian-lts-announce/2023/08/msg00026.html), fixing [CVE-2022-40982](https://security-tracker.debian.org/tracker/CVE-2022-40982), [CVE-2022-41804](https://security-tracker.debian.org/tracker/CVE-2022-41804), and [CVE-2023-23908](https://security-tracker.debian.org/tracker/CVE-2023-23908), for [intel-microcode](https://tracker.debian.org/pkg/intel-microcode).  
  For Debian 10 buster, these problems have been fixed in version 3.20230808.1~deb10u1.
- Issued [DLA 3544-1](https://lists.debian.org/debian-lts-announce/2023/08/msg00033.html), fixing [CVE-2023-20197](https://security-tracker.debian.org/tracker/CVE-2023-20197), for [clamav](https://tracker.debian.org/pkg/clamav).  
  For Debian 10 buster, these problems have been fixed in version 0.103.9+dfsg-0+deb10u1.
- Started looking at other packages.

#### ELTS Work:

- Issued [ELA 920-1](https://www.freexian.com/lts/extended/updates/ela-920-1-datatables.js/), fixing [CVE-2021-23445](https://security-tracker.debian.org/tracker/CVE-2021-23445), for [datatables.js](https://tracker.debian.org/pkg/datatables.js).  
  For Debian 9 stretch, these problems have been fixed in version 1.10.13+dfsg-2+deb9u1.  
- Issued [ELA 924-1](https://www.freexian.com/lts/extended/updates/ela-924-1-open-vm-tools/), fixing [CVE-2023-20867](https://security-tracker.debian.org/tracker/CVE-2023-20867), for [open-vm-tools](https://tracker.debian.org/pkg/open-vm-tools).  
  For Debian 8 jessie, these problems have been fixed in version 2:9.4.6-1770165-8+deb8u1.  
  For Debian 9 stretch, these problems have been fixed in version 2:10.1.5-5055683-4+deb9u4.  
- Issued [ELA 925-1](https://www.freexian.com/lts/extended/updates/ela-925-1-openssh/), fixing [CVE-2023-38408](https://security-tracker.debian.org/tracker/CVE-2023-38408), for [openssh](https://tracker.debian.org/pkg/openssh).  
  For Debian 8 jessie, these problems have been fixed in version 1:6.7p1-5+deb8u9.  
  For Debian 9 stretch, these problems have been fixed in version 1:7.4p1-10+deb9u8.  
- Issued [ELA 935-1](https://www.freexian.com/lts/extended/updates/ela-935-1-intel-microcode/), fixing [CVE-2022-40982](https://security-tracker.debian.org/tracker/CVE-2022-40982), [CVE-2022-41804](https://security-tracker.debian.org/tracker/CVE-2022-41804), and [CVE-2023-23908](https://security-tracker.debian.org/tracker/CVE-2023-23908), for [intel-microcode](https://tracker.debian.org/pkg/intel-microcode).  
  For Debian 8 jessie, these problems have been fixed in version 3.20230808.1~deb8u1.  
  For Debian 9 stretch, these problems have been fixed in version 3.20230808.1~deb9u1.  
- Issued [ELA 936-1](https://www.freexian.com/lts/extended/updates/ela-936-1-ruby-rack/), fixing [CVE-2023-27539](https://security-tracker.debian.org/tracker/CVE-2023-27539), for [ruby-rack](https://tracker.debian.org/pkg/ruby-rack).  
  For Debian 9 stretch, these problems have been fixed in version 1.6.4-4+deb9u5.  
- Issued [ELA 937-1](https://www.freexian.com/lts/extended/updates/ela-937-1-clamav/), fixing [CVE-2023-20197](https://security-tracker.debian.org/tracker/CVE-2023-20197), for [clamav](https://tracker.debian.org/pkg/clamav).  
  For Debian 8 jessie, these problems have been fixed in version 0.103.9+dfsg-0+deb8u1.  
  For Debian 9 stretch, these problems have been fixed in version 0.103.9+dfsg-0+deb9u1.  

#### Other (E)LTS Work:

- Triaged [ruby-rack](https://tracker.debian.org/pkg/ruby-rack),
  [rails](https://tracker.debian.org/pkg/rails),
  [intel-microcode](https://tracker.debian.org/pkg/intel-microcode),
  [datatables.js](https://tracker.debian.org/pkg/datatables.js),
  [open-vm-tools](https://tracker.debian.org/pkg/open-vm-tools),
  [openssh](https://tracker.debian.org/pkg/openssh),
  [clamav](https://tracker.debian.org/pkg/clamav),
  [flac](https://tracker.debian.org/pkg/flac),
  [tiff](https://tracker.debian.org/pkg/tiff),
  [trafficserver](https://tracker.debian.org/pkg/trafficserver),
  [freeimage](https://tracker.debian.org/pkg/freeimage),
  [python2.7](https://tracker.debian.org/pkg/python2.7),
  [c-ares](https://tracker.debian.org/pkg/c-ares),
  [batik](https://tracker.debian.org/pkg/batik),
  [busybox](https://tracker.debian.org/pkg/busybox),
  [cacti](https://tracker.debian.org/pkg/cacti),
  [etcd](https://tracker.debian.org/pkg/etcd),
  [gnome-gmail](https://tracker.debian.org/pkg/gnome-gmail),
  [horizon](https://tracker.debian.org/pkg/horizon),
  [iotjs](https://tracker.debian.org/pkg/iotjs),
  [libcrypto++](https://tracker.debian.org/pkg/libcrypto++),
  [libsass](https://tracker.debian.org/pkg/libsass),
  [mupdf](https://tracker.debian.org/pkg/mupdf),
  [nasm](https://tracker.debian.org/pkg/nasm),
  [opensc](https://tracker.debian.org/pkg/opensc),
  [qemu](https://tracker.debian.org/pkg/qemu),
  [qtsvg-opensource-src](https://tracker.debian.org/pkg/qtsvg-opensource-src),
  [poppler](https://tracker.debian.org/pkg/poppler),
  [tryton-server](https://tracker.debian.org/pkg/tryton-server),
  [wireshark](https://tracker.debian.org/pkg/wireshark),
  [unrar-nonfree](https://tracker.debian.org/pkg/unrar-nonfree),
  [rar](https://tracker.debian.org/pkg/rar),
  [json-c](https://tracker.debian.org/pkg/json-c), and
  [openssl](https://tracker.debian.org/pkg/openssl).
- Mark CVE-2009-1143/open-vm-tools as ignored for buster, stretch, and jessie.
- Mark CVE-2022-447{29,30}/batik as no-dsa for buster, stretch, and jessie.
- Mark CVE-2022-48174/busybox as no-dsa for buster, stretch, and jessie.
- Mark CVE-2022-41444/cacti as no-dsa for buster.
- Mark CVE-2022-34038/etcd as no-dsa for buster.
- Mark CVE-2020-24904/gnome-gmail as no-dsa for buster.
- Mark CVE-2022-45582/horizon as no-dsa for buster.
- Mark CVE-2020-24187/iotjs as ignored for buster.
- Mark CVE-2023-38961/iotjs as ignored for buster.
- Mark CVE-2022-48570/libcrypto++ as no-dsa for buster and stretch.
- Mark CVE-2022-43358/libsass as no-dsa for buster.
- Mark CVE-2020-21896/mupdf as no-dsa for buster.
- Mark CVE-2022-29654/nasm as no-das for buster and stretch.
- Mark CVE-2021-34193/opensc as no-dsa for buster.
- Mark CVE-2022-36648/qemu as postponed for buster and stretch.
- Mark CVE-2021-28025/qtsvg-opensource-src as no-dsa for buster and stretch.
- Mark poppler CVEs as no-dsa for buster, stretch, and jessie.
- Mark wireshark CVEs as no-dsa for buster and stretch.
- Mark CVE-2023-20212/clamav as not-affected for buster and bullseye.
- Mark CVE-2023-20212/clamav as not-affected for stretch and jessie.
- Mark CVE-2023-27530/ruby-rack as ignored for stretch.
- Mark CVE-2021-32292/json-c as not-affected for stretch and jessie.
- Auto EOL'd exempi, nasm, audiofile, freeimage, graphicsmagick, oggvideotools, mupdf, libraw, linux, opensc, upx-ucl, libsass, radare2, qemu, cacti, horizon, hwloc, libcrypto++, wireshark, ansible, chromium, gerbv, rar, unrar-nonfree, python-pyramid, tryton-server.
- Discussed about the ckeditor regression in stretch and jessie. Bastien kindly stepped up and rolled out a fix.
- Helped with the runc and LXC discussions on the mailing list.
- Pinged the customer about the modsecurity-crs bump.
- Participated in samba discussion a bit.
- Initiate the discussion about clamAV being EOL after 2 years and we'll have to update to 1.0.x which pulls in Rust. :)
- Helped Bastien w/ some runc vendoring bits.
- Answered questions (& discussions) on IRC (#debian-lts and #debian-elts) and Matrix.
- Participated and helped fellow members with their queries via private mail and chat.
- General and other discussions on LTS private and [public mailing list](https://lists.debian.org/debian-lts/2023/08/threads.html).
- Attended the monthly LTS meeting.

---

Until next time.  
`:wq` for today.
