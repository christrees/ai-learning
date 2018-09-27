# DevSecOps-AutomatedSecurityTesting-Overview

Notes from James Wickett class I went through

1. Security Testing Basics
    1. Security and DevOps history in short
        + Waterfall organizational structure has messed up security testing
        + Passing Audit should not equal security
        + Risk management should not equal security
    2. Security and DevOps for the first time
        + Embrase Enabling
        + See Value
        + Secure software supply chain
           1. Software Intent (secure sensitive flows)
           2. Inherit (libs and dependencies) S/W Bill of Materials (SBOM)
           3. Develop (develop for security during development)
           4. Build (Security acceptance test)
           5. Deploy (Secure config and secrets)
           6. Operate (Are you under attack, what is getting attacked)
        + Create feedback loop (in CI system pref)
    3. Automated security testing basics
        + Penetration Testing Methodology
            1. Recon
            2. Mapping
            3. Discovery
            4. Exploit
        + Automation of SAST, DAST and IAST into CI/CD
        + OpenSource Static Analysis Tools
           1. Brakeman
           2. FindBugs
        + Mapping and Inventory 
           1. Retire.js (open)
           2. Sonatype, Black Duck, Jfrog (commercial)
        + Dynamic - real tools for black
           1. Arachni
           2. Nikto
           3. ZAP
    4. Tips for security automation for DevOps
        + Don't slow down the build (builds less than 5min)
        + Split tests out if get too long
        + Bundel Sec with Perf tests (perf has the same long run test issues)
        + Don't block build/release (push to feedback system / issue)
        + Integrated into ChatOps
        + Contain thyself
2. Security Automation: Getting Started
    1. Setting up the demo environment
        + Setup Docker
        + Setup Gruyere - https://google-gruyere.appspot.com
        + https://google-gruyere.appspot.com/start/ to get a new instance
        + https://github.com/wickett/security-testing-class
    2. Web applicaiton security quick tour
    3. Application security attack tools
    4. Security test automation with Gauntit
    5. Running your first automated attack
3. Application Security Automation
    1. Application security vector: XSS
        + XSS Stored and Reflected
        + BeEF will hook web browsers to use as beachheads for browser based attacks
        + Defend XSS - Test and fix, Sanitze inputs, Encode output see OWASP.org
    2. XSS attack automation
        + Feature based attacks using tools
    3. XSS attack automation refactoring
    4. SQLi attack automation
    5. Automating a fuzzer (DIRB)
    6. Network testing on the fly (Nmap)
    7. Be mean to your code - in practice
        + Gauntlt uses Gherkin keywords
        + Gauntlt uses Aruba library (part of cucumber)
        + Gauntlt - https://github.com/gauntlt/gauntlt/tree/master/examples
4. Security Testing in Software Delivery Pipelines
    1. Shift left and the DevOps way
        + config/cucumber.yml
    2. Security testing in CI/CD
        + Setup for Travis - https://github.com/wickett/security-testing-class
6. Conclusion
    1. Start automating security testing
    2. Next Steps
    
## Resources
+ https://github.com/wickett/security-testing-class
