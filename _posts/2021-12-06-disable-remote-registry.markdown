---
title: "Disable Remote Registry via Intune Remediation"
layout: post
headerImage: false
tag:
- remediation
- powershell
- registry
- security
- service
star: true
category: blog
author: intuner
description: Intune remediation
---
## Why disable Remote Registry?
 Keeping the Remote Registry service enabled can pose a security risk. It allows remote users to modify the registry settings on your computer, which can be exploited by malicious actors to gain unauthorized access or control over your system

{% gist eed24c479d6e8f347762c46a37574939 %}
