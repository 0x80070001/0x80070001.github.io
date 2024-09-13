---
title: "Disable Fast Startup via Intune Remediation"
layout: post
headerImage: false
tag:
- remediation
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
Shutdown isn't shutdown, reboot is shutdown. Huh?!?

Fast Startup can mask underlying issues since the system isn’t really resetting on shutdown. Disabling it ensures that your computer starts fresh each time, making it easier to identify and resolve problems.

Many businesses I've worked with utilise docking stations
to provide a better user experience when roaming. Allowing an end user to connect a single cable to their laptop
to connect to multiple displays, ethernet, keyboard and mice is nice!... when it works.

I've found hibernation can cause Windows to be unreliable in this situation. I've often seen monitors fail to activate
or even fail during use. End users then begin unplugging the dock and the situation spirals.

Disabling Fast Startup (in most cases) has improved Windows reliability when using docking stations.

## Why use a Remediation?
The Intune ADMX policy does not disable fast start, it simply sets it to NOT CONFIGURED.

{% gist 4b0a3684e75db993ebd7e6138dea6727 %}
