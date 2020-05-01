+++
date = "2020-05-01"
title = "FOSS Activites in April 2020"
slug = "foss-in-april-20"
images = ["/images/debian-lts-small.png", "/images/debian-logo-small.png", "/images/ruby-logo-small.png", "/images/vendetta.jpg"]
tags = [
    "debian",
    "monthly",
]
categories = [
    "debian",
    "open-source",
]
+++

Here's my (seventh) monthly update about the activities I've done in the F/L/OSS world.

## Debian
{{< figure src="/images/debian-logo-small.png" >}}

It's been 14 months since I've started contributing to Debian.
And 4 months since I've been a Debian Developer. And in this beautiful time,
I had this opprotunity to do and learn lots of new and interesting things. And most
importantly, meet and interact with lots of lovely people! 💖  
Debian is `$home`.  

#### Uploads:

- [libgit2](https://tracker.debian.org/pkg/libgit2) (0.28.5+dfsg.1-1) - new upstream version.  
- [ruby-ffi-compiler](https://tracker.debian.org/pkg/ruby-ffi-compiler) (1.0.1-1) - NEW ([#955497](https://bugs.debian.org/#955497)).  
- [rake](https://tracker.debian.org/pkg/rake) (13.0.1-3/4) - using `--gem-install layout` and fixing autopkgtest.  
- [mcollective](https://tracker.debian.org/pkg/mcollective) (2.12.5+dfsg-1) - new upstream version.  
- [ruby-guard](https://tracker.debian.org/pkg/ruby-guard) (2.16.2-1) - fix regression caused by pry's upload ([#954724](https://bugs.debian.org/#954724)).  
- [ruby-pry-byebug](https://tracker.debian.org/pkg/ruby-pry-byebug) (3.9.0-1) - fix regression caused by pry's upload ([#954572](https://bugs.debian.org/#954572)).  
- [ruby-ahoy-matey](https://tracker.debian.org/pkg/ruby-ahoy-matey) (3.0.2-1) - new upstream version.  
- [ruby-http-parser](https://tracker.debian.org/pkg/ruby-http-parser) (1.2.1-1) - NEW ([#955589](https://bugs.debian.org/#955589)).  
- [ruby-http-parser.rb](https://tracker.debian.org/pkg/ruby-http-parser.rb) (0.6.0-5) - Drop `Conflicts` field.  
- [golang-github-awalterschulze-gographviz](https://tracker.debian.org/pkg/golang-github-awalterschulze-gographviz) (2.0.1-1) - new upstream version.  
- [ruby-ffi-yajl](https://tracker.debian.org/pkg/ruby-ffi-yajl) (2.3.1-3) - fix build in `ARM` $arch.  
- [ruby-http](https://tracker.debian.org/pkg/ruby-http) (4.4.1-1) - new upstream version (([#890075](https://bugs.debian.org/#890075) and [#858140](https://bugs.debian.org/#858140)).  
- [ruby-twitter](https://tracker.debian.org/pkg/ruby-twitter) (7.0.0-1) - new upstream version.  
- [ruby-rack](https://tracker.debian.org/pkg/ruby-rack) (2.1.1-2) - migration to unstable.  
- [ruby-rack-oauth2](https://tracker.debian.org/pkg/ruby-rack-oauth2) (1.11.0-1) - fix FTBFS.  
- [ruby-crb-blast](https://tracker.debian.org/pkg/ruby-crb-blast) (0.6.9-4) - fix regression caused by ruby-bio ([#954536](https://bugs.debian.org/#954536)).  
- [ruby-sassc-rails](https://tracker.debian.org/pkg/ruby-sassc-rails) (2.1.2-5) - Add `Breaks+Replaces` for ruby-sass-rails ([#952682](https://bugs.debian.org/#952682) and [#954544](https://bugs.debian.org/#954544)).  
- [libdbd-firebird-perl](https://tracker.debian.org/pkg/libdbd-firebird-perl) (1.32-1) - new upstream version.  
- [ruby-minitest-global-expectations](https://tracker.debian.org/pkg/ruby-minitest-global-expectations) (1.0.1-1) - NEW ([#956051](https://bugs.debian.org/#956051)).  
- [golang-github-cheekybits-genny](https://tracker.debian.org/pkg/golang-github-cheekybits-genny) (1.0.0-1) - NEW ([#956128](https://bugs.debian.org/#956128)).  
- [node-clipboard](https://tracker.debian.org/pkg/node-clipboard) (2.0.6+ds-1~bpo10+1) - backporting to buster.  
- [micro](https://tracker.debian.org/pkg/micro) (2.0.2-3) - use `cut -d'-' -f1` to just show upstream version.  
- [golang-github-go-errors-errors](https://tracker.debian.org/pkg/golang-github-go-errors-errors) (1.0.1-4) - fix build and autopkgtest ([#954521](https://bugs.debian.org/#954521)).  
- [micro](https://tracker.debian.org/pkg/micro) (2.0.2-3~bpo10+1) - backporting to buster.  
- [libgit2](https://tracker.debian.org/pkg/libgit2) (1.0.0+dfsg.1-1) - new upstream version.  
- [micro](https://tracker.debian.org/pkg/micro) (2.0.3-1) - add support for +LINE:COL flag syntax for cursor position ([#953427](https://bugs.debian.org/#953427)).  

#### Other $things:

- Attended Ruby team meeting. Logs [here](http://meetbot.debian.net/debian-ruby/2020/debian-ruby.2020-04-03-16.31.html).  
- Attended Perl team LHF. Report [here](https://lists.debian.org/debian-perl/2020/04/msg00014.html).  
- Sponsored a lot of uploads for William Desportes and Adam Cecile.  
- Mentoring for newcomers.  
- FTP Trainee reviewing.  
- Moderation of -project mailing list.  
- Applied for [DUCI project](https://wiki.debian.org/SummerOfCode2020/Projects/#SummerOfCode2020.2FApprovedProjects.2FUpstreamDownstreamCooperationInRuby.Upstream.2FDownstream_cooperation_in_Ruby) for Google Summer of Code 2020.  

---

## Ruby2.7 Migration:
{{< figure src="/images/ruby-logo-small.png" >}}

Ruby2.7 was recently released on 25th December, 2019. Santa's gift. Believe it or not.
We, the Debian Ruby team, have been trying hard to make it migrate to testing. And it finally happened.
The default version in testing is ruby2.7. Here's the [news](https://tracker.debian.org/news/1119524/ruby-defaults-1271-migrated-to-testing/)! \o/  
Here's what I worked on this month for this transition.  

#### Upstream:

Opened several issues and proposed patches (in the form of PRs):

- [Issue #35](https://github.com/attr-encrypted/encryptor/issues/35) against `encryptor` for Ruby2.7 test failures.  
- [Issue #28](https://github.com/seattlerb/image_science/issues/28) against `image_science` for removing relative paths.  
- [Issue #106](https://github.com/chef/ffi-yajl/issues/106) against `ffi-yajl` for Ruby2.7 test failures.  
- [PR #5](https://github.com/josephruscio/aggregate/pull/5) against `aggregate` for simply using `require`.  
- [PR #6](https://github.com/josephruscio/aggregate/pull/6) against `aggregate` for modernizing CI and adding Ruby 2.5 and 2.7 support.  
- [Issue #13](https://github.com/dejan/espeak-ruby/issues/13) against `espeak-ruby` for Ruby2.7 test failures.  
- [Issue #4](https://github.com/piotrmurach/tty-which/issues/4) against `tty-which` for test failures in general.  
- [Issue #11](https://github.com/marcandre/packable/issues/11) against `packable` for Ruby2.7 test failures. [PR #12](https://github.com/marcandre/packable/pull/12) has been proposed.  
- [Issue #10](https://github.com/tj/growl/issues/10) against `growl` for test failures and proposed an initial patch.  

#### Downstream:

I fixed and uploaded the following packages in Debian:

- [puppet-beaker](https://tracker.debian.org/pkg/puppet-beaker) (4.21.0-1) - new upstream version and fix FTBFS ([#956595](https://bugs.debian.org/#956595) and [#954614](https://bugs.debian.org/#954614)).  
- [ruby-fakeweb](https://tracker.debian.org/pkg/ruby-fakeweb) (1.3.0+git20170806+dfsg1-2) - fix autopkgtest ([#952042](https://bugs.debian.org/#952042)).  
- [puppet-lint](https://tracker.debian.org/pkg/puppet-lint) (2.4.2-2) - fix FTBFS for Ruby2.7 migration.  
- [ruby-hoe](https://tracker.debian.org/pkg/ruby-hoe) (3.22.1+dfsg1-1) - new upstream version and fix FTBFS ([#952041](https://bugs.debian.org/#952041)).  
- [rake-compiler](https://tracker.debian.org/pkg/rake-compiler) (1.0.5-2) - fix FTBFS.  
- [ruby-aggregate](https://tracker.debian.org/pkg/ruby-aggregate) (0.2.2-3) - fix autopkgtest.  
- [facter](https://tracker.debian.org/pkg/facter) (3.11.0-4) - fix autopkgtest ([#955582](https://bugs.debian.org/#955582)).  

---

## Debian LTS
{{< figure src="/images/debian-lts-small.png" >}}

Debian Long Term Support (LTS) is a project to extend the lifetime of all Debian stable releases
to (at least) 5 years. Debian LTS is not handled by the Debian security team, but by a separate group
of volunteers and companies interested in making it a success.  
This was my seventh month as a Debian LTS paid contributor. I was assigned 24.00 hours and worked on
the following things:  

#### CVE Fixes and Announcements:

- Issued [DLA 2178-1](https://lists.debian.org/debian-lts-announce/2020/04/msg00011.html), fixing [CVE-2020-11728](https://security-tracker.debian.org/tracker/CVE-2020-11728) and [CVE-2020-11729](https://security-tracker.debian.org/tracker/CVE-2020-11729), for [awl](https://tracker.debian.org/awl).  
  For Debian 8 "Jessie", these problems have been fixed in version 0.55-1+deb8u1.  

- Issued [DLA 2179-1](https://lists.debian.org/debian-lts-announce/2020/04/msg00012.html), fixing [CVE-2020-10968](https://security-tracker.debian.org/tracker/CVE-2020-10968), [CVE-2020-10969](https://security-tracker.debian.org/tracker/CVE-2020-10969), [CVE-2020-11111](https://security-tracker.debian.org/tracker/CVE-2020-11111),
  [CVE-2020-11112](https://security-tracker.debian.org/tracker/CVE-2020-11112), [CVE-2020-11113](https://security-tracker.debian.org/tracker/CVE-2020-11113), [CVE-2020-11619](https://security-tracker.debian.org/tracker/CVE-2020-11619), and [CVE-2020-11620](https://security-tracker.debian.org/tracker/CVE-2020-11620), for [jackson-databind](https://tracker.debian.org/jackson-databind).  
  For Debian 8 "Jessie", these problems have been fixed in version 2.4.2-2+deb8u14.  

- Issued [DLA 2180-1](https://lists.debian.org/debian-lts-announce/2020/04/msg00013.html), fixing [CVE-2020-11736](https://security-tracker.debian.org/tracker/CVE-2020-11736), for [file-roller](https://tracker.debian.org/file-roller).  
  For Debian 8 "Jessie", this problem has been fixed in version 3.14.1-1+deb8u2.  

- Issued [DLA 2190-1](https://lists.debian.org/debian-lts-announce/2020/04/msg00023.html), fixing [CVE-2020-10663](https://security-tracker.debian.org/tracker/CVE-2020-10663), for [ruby-json](https://tracker.debian.org/ruby-json).  
  For Debian 8 "Jessie", this problem has been fixed in version 1.8.1-1+deb8u1.  

#### Other LTS Work:

- Triaged [jackson-databind](https://tracker.debian.org/pkg/jackson-databind),
[libconvert-asn1-perl](https://tracker.debian.org/pkg/libconvert-asn1-perl),
[file-roller](https://tracker.debian.org/pkg/file-roller),
[awl](https://tracker.debian.org/pkg/awl),
[dom4j](https://tracker.debian.org/pkg/dom4j),
and [openvpn](https://tracker.debian.org/pkg/openvpn).  
- Mark CVE-2013-7488/libconvert-asn1-perl as no-dsa for Jessie.  
- Mark CVE-2020-11810/openvpn as no-dsa for Jessie.  
- Ping ntp's upstream for relevant commits.  
- Mark CVE-2019-16782/ruby-rack as no-dsa for Jessie.  
- Attended first LTS meeting. Logs [here](http://meetbot.debian.net/debian-lts/2020/debian-lts.2020-04-29-13.59.html).  
- General discussion on LTS [mailing list](https://lists.debian.org/debian-lts/2020/05/threads.html).  

---

## Other(s)
{{< figure src="/images/vendetta.jpg" >}}

Sometimes it gets hard to categorize work/things into a particular category.  
That's why I am writing all of those things inside this category.  
This includes two sub-categories and they are as follows.

#### Personal:

This month I could get the following things done:

- Most importantly, I finally migrated to a new website. Huge UI imporvement! \o/  
  From Jekyll to Hugo, it was not easy. But it was worth it! Many thanks to [Luiz](https://luizdepra.dev/) for writing [hugo-coder](https://github.com/luizdepra/hugo-coder/), [Clement](https://clementpannetier.dev/), and [Samyak](https://samyak-jn.tk/).  
  If you find any flaws, issues and pull requests are welcomed at [utkarsh2102/utkarsh2102.com](https://github.com/utkarsh2102/utkarsh2102.com) 🔥  
- Wrote [battery-alert](https://github.com/utkarsh2102/utsh/blob/master/battery-alert.sh), a mini-project of my own to show battery alerts at <10% and >90%.  
  Written in shell, it brings me all the satisfaction as it has saved my life on many occasions.  
  And guess what? It has more users than just myself! 😉  
  Reviews and patches are welcomed! \o/  
- Atteneded [Intro Sec Con](https://twitter.com/introseccon) and had the most fun!  
  Heard Ian's keynote and attended other talks and learned how to use WireShark! 🦈  

#### Open Source:

Again, this contains all the things that I couldn't categorize earlier.  
Opened several issues and pull requests:

- [Issue #297](https://github.com/luizdepra/hugo-coder/issues/297) against `hugo-coder`, asking to enable RSS feed for blogs.  
- [PR #316](https://github.com/luizdepra/hugo-coder/pull/316) for `hugo-coder` for fixing the above issue myself.  
- [Issue #173](https://github.com/activeadmin/arbre/issues/173) against `arbre` for requesting a release.  
- [Issue #104](https://github.com/pat/combustion/issues/104) against `combustion`, asking to relax dependency on rubocop. Fixed in this [commit](https://github.com/pat/combustion/commit/902df3252f9ae38a0f127b4ae086e0da4944b80f).  
- [Issue #16](https://github.com/ffi/ffi-compiler/issues/16) against `ffi-compiler` for requesting to fix homepage and license.  
- [Issue #57](https://github.com/awalterschulze/gographviz/issues/57) against `gographviz` for requesting a release.  
- [Issue #14](https://github.com/cboursnell/crb-blast/issues/14) against `crb-blast`, suggesting compatability with bio 2.0.x.  
- [Issue #58](https://github.com/flyerhzm/uniform_notifier/issues/58) against `uniform_notifier` for asking to drop the use of ruby-growl.  
- [PR #2072](https://github.com/polybar/polybar/pull/2072) for `polybar`, adding installation instructions on Debian systems.  

---

Until next time.  
`:wq` for today.
