+++
date = "2019-07-15"
title = "GSoC Report #2"
slug = "gsoc-report-2"
tags = [
    "debian",
    "gsoc"
]
categories = [
    "debian",
    "open-source",
]
+++

Hello there.

> I hope the next time I write a report, I'll have no twists and adventures to share.  

Yay, nothing much "adventurous" happened.  

Quick recap: My GSoC project is to package a software called
[Loomio](https://github.com/loomio/loomio/).
A little about Loomio:  
**Loomio** is a decision-making software, designed to assist groups with the
collaborative decision-making process.  
It is a free software web-application, where users can initiate discussions and
put up proposals.  

In the last 2 weeks, that is, the 3rd and the 4th week, I worked on setting up
Loomio-installer and packaged it's Ruby dependencies simulatenously.  

The following dependencies were packaged and uploaded:  
» ruby-ahoy-matey  
» ruby-aws-partitions  
» ruby-aws-sdk-core  
» ruby-aws-sdk-kms  
» ruby-aws-sdk-s3  
» ruby-aws-sigv4  
» ruby-geocoder  
» ruby-terrapin  

The following dependencies have been packaged but are yet to be uploaded:  
» ruby-cancancan  
» ruby-google-cloud-env  
» ruby-google-cloud-core  
» ruby-google-cloud-translate  

The following packages were updated and uploaded:  
» ruby-pg  
» ruby-activerecord-import  

The following dependencies have been fixed for `autopkgtest`:  
» ruby-paperclip (took a lot of time to debug :/)  
» ruby-maxminddb  

In the following process, I discovered a new option that could be passed to
`dh_ruby` - `export DH_RUBY_GEM_INSTALL_WHITELIST_APPEND`.  
This was needed for `ruby-aws-partitions` as test-suite of `ruby-paperclip`
needed `partitions.json`, thus the need. Thanks to the man page of `dh_ruby` :D  

Other than these dependencies, I tried setting up `loomio-installer`, the same
way as `diaspora-installer`. Just a few things had to be changed.  
Though I did the change it needed but I didn't quite test it yet.  
I am still figuring out a way to run the installer, hopefully `gbp` should help,
like it normall does.  

My other activities in Debian last month:  
» Participated in Perl team's LHF and updated `libfuture-asyncawait-perl`.  
» Sponsored a couple of packages (DM access).  
» Worshipping Visa God to grant visa for DebConf19.  

Plans for the next 2 weeks:  
» Testing and setting up `loomio-installer`.  
» Packaging and completing the last set of Ruby gem dependencies.  
» Prepare a list of node packages to be updated and packaged.  

I hope the next time I write a report, I'll have a better update on the
installer.  

Until next time.  
`:wq` for today.
