# DevSecOps

+ Shifting security to the left
+ DevSecOps - Overall automation of security testing in CI/CD
+ Rugged DevOps - The push of Sec patterns into the developer template lib and design process
+ Process 
   + Development - Code Review, Arch review
   + QA - Static/dynamic scan Interactive scan
   + Production - Vulnerability scanning
+ API are essential to DevOps including DevSecOps
+ Need to look at Sec tools with the API to integrate with DevOps
+ Tool Types
   + SAST - Static Application Security Testing (Fortify, AppScan, Checkmarx - FindSecBugs, Brakeman, PMD)
   + DAST - Dynamic Application Security Testing (WebInspect, Burp, AppSpider - ZAP)
   + IAST - Interactive Application Security Testing (sees code and data - Contrast, Seeker - no Open source)
+ CI/CD
+ Containers help DevSecOps by normalizing the env
+ DevSecOps Containers
   + Security test container for target app-type
   + Setup SecTool test sets in container
   + CI/CD can deploy SecTool container targets in automation
   + Use artifactory to keep build depends
+ Good DevOps includes infrastructure automation
   + Vulnerablity scanning
   + Network security group review
   + Automated patching compliance
   + Encryption at rest
+ Unified tools
   + Tools should be part of the pipeline
   + Dev = Detect
   + Ops = Detect, Protect and Block
   
## Tools
+ [Find Security Bugs](https://find-sec-bugs.github.io) - Java - https://find-sec-bugs.github.io
+ [ZAP](https://www.owasp.org) - Attack Proxy Project - https://www.owasp.org
+ [sqlmap](http://sqlmap.org) - SQL Injection - http://sqlmap.org
+ [OpenVAS](http://www.openvas.org) - Vulnerablity Scann - http://www.openvas.org
+ [Recon-ng](https://bitbucket.org/LaNMaSteR53/recon-ng) - web reconnaissance
+ [OWASP-GlueTool](https://www.owasp.org) - Docker container to glue tools together

## Reading Resources
+ A DevSecOps Playbook - by SANS Institute
+ Continuous Application Security Playbook - by Contrast Security
+ Awesome DevSecOps - at GitHub.com

## Quotes
+ Risk assessment introduces a dangerous fallacy: that structured inadequacy is almost as good as adequacy and that underfunded security efforts plus risk management are about as good as properly funded security work - Michal Zalewski
