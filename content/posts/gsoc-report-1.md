+++
date = "2019-06-15"
title = "GSoC Report #1"
slug = "gsoc-report-1"
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

The last two weeks have been adventurous. Here's what happened.  
My GSoC project is to package a software called [Loomio](https://github.com/loomio/loomio/).
A little about Loomio:  
**Loomio** is a decision-making software, designed to assist groups with the
collaborative decision-making process.  
It is a free software web-application, where users can initiate discussions and put up proposals.

Loomio is mostly written in Ruby, but also includes some CoffeeScript, Vue,
JavaScript, with a little HTML, CSS.  
The idea is to package all the dependencies of Loomio and get Loomio easily
installable on the Debian machines.  

The phase 1, that is, the first 4 weeks, were planned to package the Ruby and
the Node dependencies. When I started off, I hit an obstacle. Little did we know
about how to go about packaging complex applications like that.  
I have been helping out in packages like gitlab, diaspora, et al. And towards the
end of the last week, we learned that `loomio` needs to be done like `diaspora`.  
First goes the `loomio-installer`, then would come the main package, `loomio`.  

Now, the steps that are to be followed for `loomio-installer` are as follows:  
» Get the app source.  
» Install gem dependencies.  
» Create database.  
» Create tables/run migrations.  
» Precomiple assets (scss -> css, et al).  
» Configure nginx.  
» Start service with systemd.  
» In case of diaspora, JS front end is pulled via wrapper gems and in case of gitlab, it is pulled via npm/yarn.  
» Loomio would be done with the same way we're doing gitlab.  

Thus, in the last two weeks, the following work has been done:  
» Ruby gems' test failures patched.  
» 18 gems uploaded.  
» Looked into loomio-installer's setup.  
» Basic scripts like nginx configuration, et al written.  

My other activities in Debian last month:  
» Updated and uploaded gitlab 11.10.4 to experimental (thanks to praveen).  
» Uploaded gitaly, gitlab-workhorse.  
» Sponsored a couple of packages (DM access).  
» Learned Perl packaging and packaged 4 modules (thanks to gregoa and yadd).  
» Learned basic Python packaging.  
» Helping DC19 Bursary team (thanks to highvoltage).  
» Helping DC19 Content team (thanks to terceiro).  

Plans for the next 2 weeks:  
» Get the app source via wget (script).  
» Install gem and node dependencies via `gem install` and `npm/yarn install` (script).  
» Create database for installer.  
» Precomiple assets (scss -> css, et al).  

I hope the next time I write a report, I'll have no twists and adventures to share.  

Until next time.  
`:wq` for today.
