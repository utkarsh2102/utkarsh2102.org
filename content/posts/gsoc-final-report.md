+++
date = "2019-08-15 11:11:11 +0530"
title = "GSoC Final Report"
slug = "gsoc-final-report"
tags = [
    "debian",
    "gsoc"
]
categories = [
    "debian",
    "open-source",
]
+++

Hello, there.

> In open source, we feel strongly that to really do something well, you have to get a lot of people involved.  

Guess Linus Torvalds got that right from the start.  
While GSoC 2019 comes to end, this project hasn't. With GSoC, I started this project from scratch and I guess, this won't "die" an early age.  

Here's a quick recap:  
> My GSoC project is to package a software called
[Loomio](https://github.com/loomio/loomio/).  
> A little about it, **Loomio** is a decision-making software, designed to assist groups with the collaborative decision-making process.  
> It is a free software web-application, where users can initiate discussions and put up proposals.  

In the span of last 3 months, I worked on creating a package of Loomio for the Debian repositories. Loomio is a big, complex software to package.  
With over 484 directories and 4607 files as a part of it’s code base, it has a huge number of Ruby and Node dependencies, along with a couple of fonts that it uses.  
Out of which, around 72 ruby gems, 58 node modules, 3 fonts, and other 27 packages which were the reverse dependencies needed work. Both, including packaged and unpackaged libraries.  

Also, little did I know about the need of having `loomio-installer`.  
Thus a good amount of time went there as well (which I also talked about in my first and second report).  

---

## Work done so far!

At the time of writing this report, the following work has been done:  

#### NEW packages  

##### Packages that have been uploaded to the archive:  

» ruby-ahoy-matey  
» ruby-aws-partitions  
» ruby-aws-sdk-core  
» ruby-aws-sdk-kms  
» ruby-aws-sdk-s3  
» ruby-aws-sigv4  
» ruby-cancancan  
» ruby-data-uri  
» ruby-geocoder  
» ruby-google-cloud-core  
» ruby-google-cloud-env  
» ruby-inherited-resources  
» ruby-maxitest  
» ruby-safely-block  
» ruby-terrapin  
» ruby-memory-profiler  
» ruby-devise-i18n  
» ruby-discourse-diff  
» ruby-discriminator  
» ruby-doorkeeper-i18n  
» ruby-friendly-id  
» ruby-google-cloud-core  
» ruby-google-cloud-env  
» ruby-has-scope  
» ruby-has-secure-token  
» ruby-heroku-deflater  
» ruby-i18n-spec  
» ruby-iso  
» ruby-omniauth-openid-connect  
» ruby-paper-trail  
» ruby-referer-parser  
» ruby-safely-block  
» ruby-user-agent-parser  
» ruby-google-cloud-translate  
» ruby-maxminddb  
» ruby-omniauth-ultraauth  

##### Packages that are yet to be uploaded:  

» ruby-arbre  
» ruby-paperclip  
» ruby-ahoy-email  
» ruby-ransack  
» ruby-benchmark-memory  
» ruby-ammeter  
» ruby-rspec-tag-matchers  
» ruby-formtastic  
» ruby-formtastic-i18n  
» ruby-rails-serve-static-assets  
» ruby-activeadmin  
» ruby-rails-12factor  
» ruby-rails-stdout-logging  
» loomio-installer  

#### Updated packages  

» rails  
» ruby-devise  
» ruby-globalid  
» ruby-pg  
» ruby-activerecord-import  
» ruby-rack-oauth2  
» ruby-rugged  
» ruby-task-list  
» gem2deb  
» node-find-up  
» node-matcher  
» node-supports-color  
» node-array-union  
» node-dot-prop  
» node-flush-write-stream  
» node-irregular-plurals  
» node-loud-rejection  
» node-make-dir  
» node-tmp  
» node-strip-ansi  

--- 


## Work left!  

Whilst it is clear how big and complex Loomio is, it was not humanly possible to complete the entire package of Loomio.  
At the moment, the following tasks are remaining for this project to get close to completion:  

» Debug loomio-installer.  
» Check what all node dependencies are not really needed.  
» Package and update the needed dependencies for loomio.  
» Package loomio.  
» Fix autopkgtests (if humanly possible).  
» Maintain it for life :D

---


## Other Debian activites!  

Debian is more than just my GSoC organisation to me.  
As my NM profile says and I quote,  
> Debian has really been an amazing journey, an amazing place, and an amazing family!  

With such lovely people and teams and with my DM hat on, I have been involved with a lot more than just GSoC. In the last 3 months, my activity within Debian (other than GSoC) can be summarized as follows.

### Cloud Team  

Since I've been interested in the work they do, I joined the team recently and currently helping in packaging `image finder`.  

##### NEW packages

» python-flask-marshmallow  
» python-marshmallow-sqlalchemy

---

### Perl Team

With Gregor, Intrigeri, Yadd, Nodens, and Bremner being there, I learned Perl packaging and helped in maintaining the Perl modules.

##### NEW packages  

» libdata-dumper-compact-perl  
» libminion-backend-sqlite-perl  
» libmoox-shorthas-perl  
» libmu-perl  

##### Updated packages  

» libasync-interrupt-perl  
» libbareword-filehandles-perl  
» libcatalyst-manual-perl  
» libdancer2-perl  
» libdist-zilla-plugin-git-perl  
» libdist-zilla-plugin-makemaker-awesome-perl  
» libdist-zilla-plugin-ourpkgversion-perl  
» libdomain-publicsuffix-perl  
» libfile-find-object-rule-perl  
» libfile-flock-retry-perl  
» libgeoip2-perl  
» libgraphics-colornames-www-perl  
» libio-aio-perl  
» libio-async-perl  
» libmail-box-perl  
» libmail-chimp3-perl  
» libmath-clipper-perl  
» libminion-perl  
» libmojo-pg-perl  
» libnet-amazon-s3-perl  
» libnet-appliance-session-perl  
» libnet-cli-interact-perl  
» libnet-frame-perl  
» libnetpacket-perl  
» librinci-perl  
» libperl-critic-policy-variables-prohibitlooponhash-perl  
» libsah-schemas-rinci-perl  
» libstrictures-perl  
» libsisimai-perl  
» libstring-tagged-perl  
» libsystem-info-perl  
» libtex-encode-perl  
» libxxx-perl

---


### Python Team  

Since I lately learned Python packaging, there are a couple of packages that I worked on which I haven't pushed yet, but by later this month.  

» python3-dotenv  
» python3-phonenumbers  
» django-phonenumber-field  
» django-phone-verify  
» Helping newbies (thanks to DC19 talk).

---

### JavaScript Team  

Super thanks to Xavier (yadd) and Praveen for being right there. Worked on the following things.  

» Helping in webpack transition (bit).  
» Helping in nodejs transition.  
» Helping in complying pkg-js-tools in all packages.  
» Packaging dependencies of ava.  
» node-d3-request   
» node-find-up  
» node-matcher  
» node-supports-color  
» node-array-union  
» node-dot-prop  
» node-flush-write-stream  
» node-irregular-plurals  
» node-loud-rejection  
» node-make-dir  
» node-tmp  
» node-strip-ansi  

---

### Golang Team  

I joined the Golang team to mostly help in doing the GitLab stuff. Thus did the following things.  

» gitlab-workhorse  
» gitaly  
» Upstream contribution to gitaly.  

---

### Ruby Team  

This is where I started from. All thanks to Praveen, Abhijith, and Raju.  
In the last 3 months, except for maintaining packages for Loomio, I did the following things.  

» Helping in maintaining GitLab (one of the maintainers).  
» Setting the fasttrack repo; announcements soon!  
» Fixing gem2deb for adding d/upstream/metadata.  
» Enabling Salsa CI for 1392 packages (yes, I broke salsa :/).  
» Reviewing and sponsoring packages.  
» Co-chairing the Ruby Team BoF.  
» And others.  

---

### Others

» Part of DC19 Content Team (thanks to Antonio).  
» Part of DC19 Bursary Team (thanks to Jonathan).  
» Perl sprint (DebCamp).  
» Newbie's Perspective Towards Debian talk (Open day).  
» Chairing Ruby Team BoF.  
» Presenting my GSoC project.  
» Part of DC19 Video Team.  
» Talking about Debian elsewhere (cf: [mail archive](http://lists.dgplug.org/pipermail/users-dgplug.org/2019-August/001948.html)).  
» DC21 Indian bid ;)  
» Organising MiniDebConf Goa :D

---

### Acknowledgement :)

> Never forget your roots.

And I haven't. The last 8 months with Debian have been super amazing. Nothing I'd like to change, even if I could. Every person here is a mentor to me.  
But above all, there are a couple of people who helped me immensely.  
Starting with Pirate Praveen, Rajudev, Abhijith, Sruthi, Gregor, Xavier, Intrigeri, Nodens, Holger, Antonio Terceiro, Kanashiro, Boutil, Georg, Sanyam, Sakshi, Jatin, and Samyak.
And of course, my little brother, Aryan.  
Sorry if I'm forgetting anyone. Thank y'all :)

NOTE: Sorry for making this extremely long; someone told me to put in all the crap I did in last 90 days :P  
Also, sorry if it gets too long on planet.d.o. :)


Until next time.  
`:wq` for today.
