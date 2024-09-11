---
title: "Why you may want to disable Fast Startup on Windows"
layout: post
date: 2021-12-02 20:00
headerImage: false
tag:
- powershell
- registry
star: true
category: blog
author: intuner
description: Intune remediation
---
## What is Fast Startup?

Fast Startup is a feature in Windows designed to reduce the time it takes for your computer to boot. While this sounds great in theory, there are several reasons why you might want to consider disabling it.

## Why disable Fast Startup?
Fast Startup can prevent Windows from applying updates correctly. When you shut down your computer with Fast Startup enabled, it doesn’t fully close all processes, which can interfere with the installation of updates and system maintenance tasks.

## Why I've disabled it?
Make troubleshooting easier, ifenabled, Fast Startup can mask underlying issues since the system isn’t really resetting. Disabling it ensures that your computer starts fresh each time, making it easier to identify and resolve problems.

Many businesses I've worked with utilise docking stations
to provide a better user experience when roaming. Allowing an end user to connect a single cable to their laptop
to connect to multiple displays, ethernet, keyboard and mice is nice!... when it works.

I've found hibernation can cause Windows to be unreliable in this situation. I've often seen monitors fail to activate
or even fail during use. End users then begin unplugging the dock and the situation spirals.

Disabling Fast Startup (in most cases) has improved Windows reliability when using docking stations.

{% gist 4b0a3684e75db993ebd7e6138dea6727 %}
