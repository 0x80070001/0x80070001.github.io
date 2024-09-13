---
title: "Disable NetFx3 (.NET Framework 3.5) in Windows via Intune Remediation"
layout: post
headerImage: false
tag:
- remediation
- powershell
- security
- WindowsOptionalFeature
star: true
category: blog
author: intuner
description: Intune remediation
---
## Why disable NetFX3?
Older versions of .NET Framework may have vulnerabilities that could be exploited by malicious software. Disabling it can help reduce the attack surface on your system.

{% gist 53f4aead8b48979f0b5b9ff63f5dd624 %}
