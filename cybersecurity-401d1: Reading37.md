Mario Pugh    November 24, 2020

OWASP ZAP

Security Testing Basics

Software security testing is the process of assessing and testing a system to discover security risks and vulnerabilities of the system and its data. While there is no universal terminology OWASP defines assessments as the analysis and discovery of vulnerabilities without attempting to actually exploit those vulnerabilities. Testing as the discovery and attempted exploitation of vulnerabilities.

Security testing is often broken out, somewhat arbitrarily, according to either the type of vulnerability being tested or the type of testing being done. A common breakout is:

Vulnerability Assessment – The system is scanned and analyzed for security issues.
Penetration Testing – The system undergoes analysis and attack from simulated malicious attackers.
Runtime Testing – The system undergoes analysis and security testing from an end-user.
Code Review – The system code undergoes a detailed review and analysis looking specifically for security vulnerabilities.

Pen Testing Basics

Both manual and automated pentesting are used, often in conjunction, to test everything from servers, to networks, to devices, to endpoints. 

Pentesting usually follows these stages:

Explore – The tester attempts to learn about the system being tested. This includes trying to determine what software is in use, what endpoints exist, what patches are installed, etc. It also includes searching the site for hidden content, known vulnerabilities, and other indications of weakness.
Attack – The tester attempts to exploit the known or suspected vulnerabilities to prove they exist.
Report – The tester reports back the results of their testing, including the vulnerabilities, how they exploited them and how difficult the exploits were, and the severity of the exploitation.
