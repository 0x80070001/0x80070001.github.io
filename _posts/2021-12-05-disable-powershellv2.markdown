---
title: "Disable PowerShell V2 via Intune Remediation"
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
## Why disable PowerShell V2?
This version of powershell is susceptible to remote code execution vulnerabilities and it
does not support Constrained Language Mode!

{% gist fb21b3de1b41f8abac28b17bae33afc3 %}
