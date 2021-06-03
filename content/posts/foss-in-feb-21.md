+++
date = "2021-03-01 20:00:00 +0530"
title = "FOSS Activites in February 2021"
slug = "foss-in-feb-21"
images = [
    "/images/debian-logo-small.png",
    "/images/debian_ruby.png",
    "/images/ruby-logo-small.png",
    "/images/debian-lts-small.png",
    "/images/computing.jpg",
    "/images/server-team-meeting.png"
]
tags = [
    "debian",
    "monthly",
]
categories = [
    "debian",
    "open-source",
]
+++

Here's my (seventeenth) monthly update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

This was my 26th month of active contributing to [Debian](https://www.debian.org/).
I became a [DM](https://wiki.debian.org/DebianMaintainer) in late March 2019 and a [DD](https://wiki.debian.org/DebianDeveloper) on Christmas '19! \o/

This month was a nice mix of amusement, excitement, nervousness, and craziness. More on it below.  
Anyway, whilst I was super-insanely busy this month, I still did some Debian stuff here and there. Here are the following things I worked on:

#### Uploads and bug fixes:

- [ruby-mechanize](https://tracker.debian.org/pkg/ruby-mechanize) (2.7.7-1) - Fixing [CVE-2021-21289](https://security-tracker.debian.org/tracker/CVE-2021-21289).
- [rails](https://tracker.debian.org/pkg/rails) (2:6.0.3.4+dfsg-3) - Fixing silent build failure, [bug #979133](https://bugs.debian.org/979133).
- [tiledb](https://tracker.debian.org/pkg/tiledb) (1.7.7-1.1) - NMU + source-only upload for migration.
- [ruby-launchy](https://tracker.debian.org/pkg/ruby-launchy) (2.5.0-3) - Add Breaks+Replaces for launchy; fixing [bug #974046](https://bugs.debian.org/974046).
- [ruby-upr](https://tracker.debian.org/pkg/ruby-upr) (0.3.0-3) - Fixing FTBFS + autopkgtest; cf: [bug #883370](https://bugs.debian.org/883370).
- [gdisk](https://tracker.debian.org/pkg/gdisk) (1.0.6-1.1) - Add Restrictions: allow-stderr for autopkgtest; fixing [bug #981231](https://bugs.debian.org/981231).
- [test-check-clojure](https://tracker.debian.org/pkg/test-check-clojure) (0.9.0-4) - Fixing FTBFS + autpkgtest; cf: [bug #982721](https://bugs.debian.org/982721).
- [rails](https://tracker.debian.org/pkg/rails) (2:6.0.3.5+dfsg-1) - Fixing [CVE-2021-22880](https://security-tracker.debian.org/tracker/CVE-2021-22880) and [CVE-2021-22881](https://security-tracker.debian.org/tracker/CVE-2021-22881).
- [ruby-mechanize](https://tracker.debian.org/pkg/ruby-mechanize) (2.7.6-1+deb10u1) - pu-upload, fixing [CVE-2021-21289](https://security-tracker.debian.org/tracker/CVE-2021-21289).
- [ruby-handlebars-assets](https://tracker.debian.org/pkg/ruby-handlebars-assets) (2:0.23.8+dfsg-3) - Fixing autpkgtest by embedding a dummy rails app.
- [ruby-rails-assets-emojione](https://tracker.debian.org/pkg/ruby-rails-assets-emojione) (2.2.6-5) - Fixing autpkgtest by embedding a dummy rails app.
- [ruby-rails-assets-jquery-colorbox](https://tracker.debian.org/pkg/ruby-rails-assets-jquery-colorbox) (1.6.3~dfsg-7) - Fixing autpkgtest by embedding a dummy rails app.
- [ruby-rails-assets-jquery.slimscroll](https://tracker.debian.org/pkg/ruby-rails-assets-jquery.slimscroll) (1.3.6+dfsg-3) - Fixing autpkgtest by embedding a dummy rails app.
- [ruby-rails-assets-markdown-it](https://tracker.debian.org/pkg/ruby-rails-assets-markdown-it) (8.4.2-5) - Fixing autpkgtest by embedding a dummy rails app.
- [ruby-mousetrap-rails](https://tracker.debian.org/pkg/ruby-mousetrap-rails) (1.4.6-7) - Fixing autpkgtest by embedding a dummy rails app.
- [ruby-rails-assets-jquery-fullscreen-plugin](https://tracker.debian.org/pkg/ruby-rails-assets-jquery-fullscreen-plugin) (0.5.0+dfsg-4) - Fixing autpkgtest by embedding a dummy rails app.

#### Other $things:

- Attended the Debian LTS team meeting.
- Mentoring for newcomers.
- Moderation of -project mailing list.
- Sponsored `ruby-rspec-stubbed-env` for Cédric Boutillier, heh :P

---

## Interesting Bits!

- Last month, I wrote:

  > Besides, there's something more that is in the pipelines. Can't talk about it now, shh. But
  > hopefully very sooooooon!

  And now I *can* talk about it! So here it is..  
  I've joined Canonical as a SDE to work on Ubuntu, full time!!! \o/  
  Fully remote + dream job/work + most of the work is in the open-source domain + the **beessstttt** co-workers one could ever ask for! 💖  

  It's been an amazing time so far and I'll talk more about it later this month.  
  But for now, here's our *team monitor selfie*™ (with Rick missing because of his "secret plan"! 🤦‍♂️)  
  ![](/images/server-team-meeting.png#center)  
  *We'll soon e-meet them in a more detailed manner in the next blog post, that is, later this month!*

- In another exciting news, I got 2 more CVEs assigned!!! \o/  
  No, it is not something that I found, it was discovered by Tavis Ormandy. I just assigned
  them a CVE ID, [CVE-2021-26937](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2021-26937)
  for screen and [CVE-2021-27135](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2021-27135) for xterm.  
  This is my 2nd and 3rd, so I am (still) very excited about this! ^_^

---

## Debian (E)LTS
{{< figure src="/images/debian-lts-small.png" >}}

[Debian Long Term Support (LTS)](https://www.freexian.com/en/services/debian-lts.html) is a project to extend the lifetime of all Debian stable releases to (at least) 5 years. Debian LTS is not handled by the Debian security team, but by a separate group of volunteers and companies interested in making it a success.  

And [Debian Extended LTS (ELTS)](https://deb.freexian.com/extended-lts) is its sister project, extending support to the Jessie release (+2 years after LTS support).

This was my sixteenth month as a Debian LTS and eighth month as a Debian ELTS paid contributor.  
I was assigned 60.00 hours for LTS and 60.00 hours for ELTS and worked on the following things:  
(however, I had overworked for 9 hours for both, LTS and ELTS, last month so I had to work for 51 hours for both this month!)

#### LTS CVE Fixes and Announcements:

- Issued [DLA 2544-1](https://lists.debian.org/debian-lts-announce/2021/02/msg00005.html), fixing [CVE-2020-36221](https://security-tracker.debian.org/tracker/CVE-2020-36221), [CVE-2020-36222](https://security-tracker.debian.org/tracker/CVE-2020-36222), [CVE-2020-36223](https://security-tracker.debian.org/tracker/CVE-2020-36223), [CVE-2020-36224](https://security-tracker.debian.org/tracker/CVE-2020-36224), [CVE-2020-36225](https://security-tracker.debian.org/tracker/CVE-2020-36225), [CVE-2020-36226](https://security-tracker.debian.org/tracker/CVE-2020-36226), [CVE-2020-36227](https://security-tracker.debian.org/tracker/CVE-2020-36227), [CVE-2020-36228](https://security-tracker.debian.org/tracker/CVE-2020-36228), [CVE-2020-36229](https://security-tracker.debian.org/tracker/CVE-2020-36229), and [CVE-2020-36230](https://security-tracker.debian.org/tracker/CVE-2020-36230), for [openldap](https://tracker.debian.org/pkg/openldap).  
  For Debian 9 stretch, these problems have been fixed in version 2.4.44+dfsg-5+deb9u7.
- Issued [DLA 2545-1](https://lists.debian.org/debian-lts-announce/2021/02/msg00006.html), fixing [CVE-2020-8020](https://security-tracker.debian.org/tracker/CVE-2020-8020) and [CVE-2020-8021](https://security-tracker.debian.org/tracker/CVE-2020-8021), for [open-build-service](https://tracker.debian.org/pkg/open-build-service).  
  For Debian 9 stretch, these problems have been fixed in version 2.7.1-10+deb9u1.
- Issued [DLA 2546-1](https://lists.debian.org/debian-lts-announce/2021/02/msg00007.html), fixing [CVE-2020-8695](https://security-tracker.debian.org/tracker/CVE-2020-8695), [CVE-2020-8696](https://security-tracker.debian.org/tracker/CVE-2020-8696), and [CVE-2020-8698](https://security-tracker.debian.org/tracker/CVE-2020-8698), for [intel-microcode](https://tracker.debian.org/pkg/intel-microcode).  
  For Debian 9 stretch, these problems have been fixed in version 3.20201118.1~deb9u1.
- Issued [DLA 2548-1](https://lists.debian.org/debian-lts-announce/2021/02/msg00009.html), fixing [CVE-2020-35502](https://security-tracker.debian.org/tracker/CVE-2020-35502), [CVE-2021-20209](https://security-tracker.debian.org/tracker/CVE-2021-20209), [CVE-2021-20210](https://security-tracker.debian.org/tracker/CVE-2021-20210), [CVE-2021-20211](https://security-tracker.debian.org/tracker/CVE-2021-20211), [CVE-2021-20212](https://security-tracker.debian.org/tracker/CVE-2021-20212), [CVE-2021-20213](https://security-tracker.debian.org/tracker/CVE-2021-20213), [CVE-2021-20215](https://security-tracker.debian.org/tracker/CVE-2021-20215), [CVE-2021-20216](https://security-tracker.debian.org/tracker/CVE-2021-20216), and [CVE-2021-20217](https://security-tracker.debian.org/tracker/CVE-2021-20217), for [privoxy](https://tracker.debian.org/pkg/privoxy).  
  For Debian 9 stretch, these problems have been fixed in version 3.0.26-3+deb9u1.
- Issued [DLA 2549-1](https://lists.debian.org/debian-lts-announce/2021/02/msg00010.html), fixing [CVE-2020-0256](https://security-tracker.debian.org/tracker/CVE-2020-0256) and [CVE-2021-0308](https://security-tracker.debian.org/tracker/CVE-2021-0308), for [gdisk](https://tracker.debian.org/pkg/gdisk).  
  For Debian 9 stretch, these problems have been fixed in version 1.0.1-1+deb9u1.
- Released a [non-maintainer upload](https://tracker.debian.org/news/1230167/accepted-gdisk-106-11-source-into-unstable/), fixing [#981231](https://bugs.debian.org/981231), autopkgtest regression for [CVE-2020-0256](https://security-tracker.debian.org/tracker/CVE-2020-0256) and [CVE-2021-0308](https://security-tracker.debian.org/tracker/CVE-2021-0308), for [gdisk](https://tracker.debian.org/pkg/gdisk).  
  For Debian sid, these problems have been fixed in version 1.0.6-1.1. 
- Issued [DLA 2554-1](https://lists.debian.org/debian-lts-announce/2021/02/msg00015.html), fixing [CVE-2021-26910](https://security-tracker.debian.org/tracker/CVE-2021-26910), for [firejail](https://tracker.debian.org/pkg/firejail).  
  For Debian 9 stretch, these problems have been fixed in version 0.9.44.8-2+deb9u2.
- Issued [DLA 2558-1](https://lists.debian.org/debian-lts-announce/2021/02/msg00019.html), fixing [CVE-2021-27135](https://security-tracker.debian.org/tracker/CVE-2021-27135), for [xterm](https://tracker.debian.org/pkg/xterm).  
  For Debian 9 stretch, these problems have been fixed in version 327-2+deb9u1.
- Issued [DLA 2561-1](https://lists.debian.org/debian-lts-announce/2021/02/msg00021.html), fixing [CVE-2021-21289](https://security-tracker.debian.org/tracker/CVE-2021-21289), for [ruby-mechanize](https://tracker.debian.org/pkg/ruby-mechanize).  
  For Debian 9 stretch, these problems have been fixed in version 2.7.5-1+deb9u1.
- Released [buster-pu update](https://tracker.debian.org/pkg/ruby-mechanize), fixing [CVE-2021-21289](https://security-tracker.debian.org/tracker/CVE-2021-21289), for [ruby-mechanize](https://tracker.debian.org/pkg/ruby-mechanize).  
  For Debian 10 Buster, these problems have been fixed in version 2.7.6-1+deb10u1.
- Released [team/maintainer upload](https://tracker.debian.org/news/1227462/accepted-ruby-mechanize-277-1-source-into-unstable/), fixing [CVE-2021-21289](https://security-tracker.debian.org/tracker/CVE-2021-21289), for [ruby-mechanize](https://tracker.debian.org/pkg/ruby-mechanize).  
  For Debian sid, these problems have been fixed in version 2.7.7-1.
- Released [team/maintainer upload](https://tracker.debian.org/news/1231598/accepted-rails-26035dfsg-1-source-into-unstable/), fixing [CVE-2021-22880](https://security-tracker.debian.org/tracker/CVE-2021-22880) and [CVE-2021-22881](https://security-tracker.debian.org/tracker/CVE-2021-22881), for [rails](https://tracker.debian.org/pkg/rails).  
  For Debian sid, these problems have been fixed in version 2:6.0.3.5+dfsg-1.
- Issued [DLA 2570-1](https://lists.debian.org/debian-lts-announce/2021/02/msg00031.html), fixing [CVE-2021-26937](https://security-tracker.debian.org/tracker/CVE-2021-26937), for [screen](https://tracker.debian.org/pkg/screen).  
  For Debian 9 stretch, these problems have been fixed in version 4.5.0-6+deb9u1.
- Issued [DLA 2573-1](https://lists.debian.org/debian-lts-announce/2021/02/msg00034.html), fixing [#981404](https://bugs.debian.org/981404) and [#982519](https://bugs.debian.org/982519), for [libzstd](https://tracker.debian.org/pkg/libzstd).  
  For Debian 9 stretch, these problems have been fixed in version 1.1.2-1+deb9u1.
- Issued [DLA 2574-1](https://lists.debian.org/debian-lts-announce/2021/02/msg00035.html), fixing [CVE-2021-27212](https://security-tracker.debian.org/tracker/CVE-2021-27212), for [openldap](https://tracker.debian.org/pkg/openldap).  
  For Debian 9 stretch, these problems have been fixed in version 2.4.44+dfsg-5+deb9u8.

#### ELTS CVE Fixes and Announcements:

- Issued [ELA 357-1](https://deb.freexian.com/extended-lts/updates/ela-357-1-jasper/), fixing [CVE-2021-3272](https://security-tracker.debian.org/tracker/CVE-2021-3272), for [jasper](https://tracker.debian.org/pkg/jasper).  
  For Debian 8 jessie, these problems have been fixed in version 1.900.1-debian1-2.4+deb8u7.
- Issued [ELA 358-1](https://deb.freexian.com/extended-lts/updates/ela-358-1-openldap/), fixing [CVE-2020-36221](https://security-tracker.debian.org/tracker/CVE-2020-36221), [CVE-2020-36222](https://security-tracker.debian.org/tracker/CVE-2020-36222), [CVE-2020-36223](https://security-tracker.debian.org/tracker/CVE-2020-36223), [CVE-2020-36224](https://security-tracker.debian.org/tracker/CVE-2020-36224), [CVE-2020-36225](https://security-tracker.debian.org/tracker/CVE-2020-36225), [CVE-2020-36226](https://security-tracker.debian.org/tracker/CVE-2020-36226), [CVE-2020-36227](https://security-tracker.debian.org/tracker/CVE-2020-36227), [CVE-2020-36228](https://security-tracker.debian.org/tracker/CVE-2020-36228), [CVE-2020-36229](https://security-tracker.debian.org/tracker/CVE-2020-36229), and [CVE-2020-36230](https://security-tracker.debian.org/tracker/CVE-2020-36230), for [openldap](https://tracker.debian.org/pkg/openldap).  
  For Debian 8 jessie, these problems have been fixed in version 2.4.40+dfsg-1+deb8u9.
- Issued [ELA 359-1](https://deb.freexian.com/extended-lts/updates/ela-359-1-python-apt/), fixing [CVE-2020-27351](https://security-tracker.debian.org/tracker/CVE-2020-27351), for [python-apt](https://tracker.debian.org/pkg/python-apt).  
  For Debian 8 jessie, these problems have been fixed in version 0.9.3.14.
- Issued [ELA 360-1](https://deb.freexian.com/extended-lts/updates/ela-360-1-gdisk/), fixing [CVE-2020-0256](https://security-tracker.debian.org/tracker/CVE-2020-0256) and [CVE-2021-0308](https://security-tracker.debian.org/tracker/CVE-2021-0308), for [gdisk](https://tracker.debian.org/pkg/gdisk).  
  For Debian 8 jessie, these problems have been fixed in version 0.8.10-2+deb8u1.
- Issued [ELA 361-1](https://deb.freexian.com/extended-lts/updates/ela-361-1-jasper/), fixing [CVE-2021-26926](https://security-tracker.debian.org/tracker/CVE-2021-26926) and [CVE-2021-26927](https://security-tracker.debian.org/tracker/CVE-2021-26927), for [jasper](https://tracker.debian.org/pkg/jasper).  
  For Debian 8 jessie, these problems have been fixed in version 1.900.1-debian1-2.4+deb8u9.
- Issued [ELA 362-1](https://deb.freexian.com/extended-lts/updates/ela-362-1-intel-microcode/), fixing [CVE-2020-8695](https://security-tracker.debian.org/tracker/CVE-2020-8695), [CVE-2020-8696](https://security-tracker.debian.org/tracker/CVE-2020-8696), and [CVE-2020-8698](https://security-tracker.debian.org/tracker/CVE-2020-8698), for [intel-microcode](https://tracker.debian.org/pkg/intel-microcode).  
  For Debian 8 jessie, these problems have been fixed in version 3.20201118.1~deb8u1.
- Issued [ELA 363-1](https://deb.freexian.com/extended-lts/updates/ela-363-1-xterm/), fixing [CVE-2021-27135](https://security-tracker.debian.org/tracker/CVE-2021-27135), for [xterm](https://tracker.debian.org/pkg/xterm).  
  For Debian 8 jessie, these problems have been fixed in version 312-2+deb8u1.
- Issued [ELA 371-1](https://deb.freexian.com/extended-lts/updates/ela-371-1-openldap/), fixing [CVE-2021-27212](https://security-tracker.debian.org/tracker/CVE-2021-27212), for [openldap](https://tracker.debian.org/pkg/openldap).  
  For Debian 8 jessie, these problems have been fixed in version 2.4.40+dfsg-1+deb8u10.

#### Other (E)LTS Work:

- Front-desk duty from 22-02 until 28-02 for both LTS and ELTS.
- Triaged [privoxy](https://tracker.debian.org/pkg/privoxy),
[dnsmasq](https://tracker.debian.org/pkg/dnsmasq),
[openldap](https://tracker.debian.org/pkg/openldap),
[libzstd](https://tracker.debian.org/pkg/libzstd),
[ruby-mechanize](https://tracker.debian.org/pkg/ruby-mechanize),
[firefox-esr](https://tracker.debian.org/pkg/firefox-esr),
[thunderbird](https://tracker.debian.org/pkg/thunderbird),
[screen](https://tracker.debian.org/pkg/screen),
[xterm](https://tracker.debian.org/pkg/xterm),
[glibc](https://tracker.debian.org/pkg/glibc),
[isync](https://tracker.debian.org/pkg/isync),
[rails](https://tracker.debian.org/pkg/rails),
[openscad](https://tracker.debian.org/pkg/openscad),
[imagemagick](https://tracker.debian.org/pkg/imagemagick),
[avahi](https://tracker.debian.org/pkg/avahi),
[gdk-pixbuf](https://tracker.debian.org/pkg/gdk-pixbuf),
[python-reportlab](https://tracker.debian.org/pkg/python-reportlab),
[python-aiohttp](https://tracker.debian.org/pkg/python-aiohttp),
[spip](https://tracker.debian.org/pkg/spip),
[gdisk](https://tracker.debian.org/pkg/gdisk), and
[jasper](https://tracker.debian.org/pkg/jasper).
- Marked CVE-2021-20214/privoxy as not-affected for stretch.
- Marked CVE-2021-27645/glibc as no-dsa for stretch.
- Marked CVE-2021-20247/isync as no-dsa for stretch.
- Marked CVE-2020-28599/openscad as no-dsa for stretch.
- Markec CVE-2021-2024{1,4-6}/imagemagick as ignored for stretch.
- Marked CVE-2021-26720/avahi as postponed for jessie.
- Marked CVE-2021-20240/gdk-pixbuf as not-affected for jessie.
- Marked CVE-2021-27645/glibc as no-dsa for jessie.
- Marked CVE-2020-28463/python-reportlab as postponed for jessie.
- Document extra CVEs as notes for imagemagick in jessie.
- Auto EOL'ed libupnp, webkit2gtk, libraw, jackson-dataformat-cbor, node-lodash, linux, asterisk, yara, python-django, botan1.10, smarty3, xen, u-boot, steghide, mumble, gsoap, ruby-twitter-stream, isync, nodejs, openscad, mupdf, mongo-java-driver, firefox-esr, thunderbird, and salt for jessie.
- Sponsored upload for php-horde-text-filter for Sylvain and published its DLA announcement.
- Got [CVE-2021-26937](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2021-26937) for [screen](https://www.gnu.org/software/screen/). Yay, this is the 2nd one I got assigned! \o/
- Got [CVE-2021-27135](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2021-27135) for [xterm](https://invisible-island.net/xterm/). Woah, this is the 3rd one, am I on a roll or what? \o/
- Co-ordinated with package maintainer (and upstream) of ca-certificates for backporting patch to stretch.
- Co-ordinated with package maintainer of ca-certificates for backporting patch to stretch.
- Co-ordinated with package maintainer of screen for fixing vulnerabilites in stretch.
- Attended monthly meeting for Debian LTS.
- Answered questions (& discussions) on IRC (#debian-lts and #debian-elts).
- Cross-checked LTS survey results, emailed Ola about the problems found.
- General and other discussions on LTS private and [public mailing list](https://lists.debian.org/debian-lts/2021/02/threads.html).

---

Until next time.  
`:wq` for today.
