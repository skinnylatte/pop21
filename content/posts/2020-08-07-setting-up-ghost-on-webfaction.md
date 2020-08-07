---
title: Setting up Ghost on Webfaction
date: 2020-08-07T03:55:49.992Z
description: If you must used shared hosting, Webfaction is still not a bad
  choice. Their Ghost installer helps you set up the popular publishing tool
  easily. Too bad their documentation is not great.
tags:
  - ghost
  - blog
  - tech
  - cms
---
I have had a Webfaction account for a long time. I keep random projects on it. In most things I have moved on to other services, but it's still useful once in a while given that for the low price I can keep a lot of crap on it.

Recently, I wanted to install [Ghost](https://ghost.org) as a headless CMS on another project. I had a thought that it might be easy to set up on my shared hosting than to try to set it up on my own dedicated server. Indeed, it was.

**Log in to Webfaction dashboard**

For most users, you can login to [my.webfaction.com](https://my.webfaction.com).

**Add the Ghost and Node applications**

* From the dashboard, click Domains/Websites then Applications
* Add two applications: Ghost, and Node.

**Set up website**

* Navigate to Websites.
* Add a website. Name it whatever you want
* Add the domains you want to use (make sure you point your domain to your Webfaction server's IP address)
* Click reuse applications, be sure to select the Node and Ghost apps you just created
* Select the https settings you prefer (I use LetsEncrypt and highly recommend it, though Webfaction's shared certificate works just fine)
* It will prompt you for a path for Ghost. I selected mydomain.tld/ghost
* Click save
* Give it a few seconds, and browse to mydomain.tld/ghost (with https if you selected that)

Follow the on-screen instructions to complete the installation and log in!