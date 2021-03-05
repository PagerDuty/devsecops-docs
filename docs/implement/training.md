![Training for Engineers](../assets/img/headers/training.png)

## Threat Modeling Exercises

This is similar to the exercises that developers and operators do for production, such as running chaos experiments (at PagerDuty we’ve been doing [Failure Fridays](https://www.pagerduty.com/blog/failure-friday-at-pagerduty/) for [years](https://www.pagerduty.com/blog/failure-fridays-four-years/)). These exercises allow teams of both disciplines to really understand the interdependencies of our complex systems. Threat modeling is a similar idea. The goal of threat modeling is to consider the security implications of your environment, including but not limited to the code written, the services running, and overall test coverage. In the DevSecOps model, at a minimum, you’ll need all three teams—development, operations, and security—to gather and contribute within their areas of expertise. 

But how do you get started? Take a look at the [STRIDE](https://en.wikipedia.org/wiki/STRIDE_(security)) framework for threat modeling. The acronym stands for:

* **Spoofed identity**
    * This is when someone who does not have an identity is able to access that identity, for example a sysadmin identity, usually to take advantage of resources and/or data that it has access to.
* **Tampering with input**
    * Modifying data that has been sent to a system.
* **Repudiation of action**
    * Non-repudiation is, generically, the inability to dispute who authored something, or who performed an action. In the context of IT,, this mostly comes up in signatures and audit trails. You want to ensure that logs cannot be tampered with, so you can always ensure that whatever entity is logged as performing an action, did that action, and that actions are logged.
* **Information disclosure**
    * When someone is able to access information they should not be able to, like an individual customer’s address (e.g. spoofing as that customer) or payment information, among other things.
* **Denial of service**
    * This is when a service, system, or application is flooded with traffic or information with the intent to bring it down (i.e. to deny service).
* **Escalation of privilege**
    * When a user or account is able to gain more access to a service, system, or application than was intended by design.

ThoughtWorks, a software consultancy, created cue cards and other materials to assist if you are interested in using STRIDE. You can find them on their Agile Threat Modeling site [here](https://thoughtworksinc.github.io/sensible-security-conversations/). It’s important to recognize, as mentioned above, that STRIDE is not a complete threat modeling framework, it is a starting point. Some points to consider not covered by STRIDE are how to handle the discovered vulnerabilities, how to rank their risk, how to ensure the resulting work is appropriately prioritized in the backlog, and so forth. To get started with all of these, you’ll be working with your security team and I also recommend leveraging OWASP and NIST materials for additional insight.

Running a threat modeling session is a lot like other deep-dive meetings, like [postmortems](https://postmortems.pagerduty.com/meeting/) and [retrospectives](https://retrospectives.pagerduty.com/planning/). The goal is to have a meeting that is long enough, while avoiding running too long. Since these meetings are exercises to improve your security posture and mindset, you’ll also want to make sure that you have them on a regular basis. To get started with both, try one hour sessions every other week and iterate from there until you find what works best for your team. Remember that time boxing is important to help everyone retain and put into practice what they have learned. For pacing, make sure the meetings are close enough together that you can continue in the next meeting rather than be tempted to “go into overtime” in your current session.

## Capture the Flag Games

The digital version of the grade school game! A quick recap of the land version for the unfamiliar: capture the flag (CTF) is a game where you capture an item (usually a piece of cloth representing a flag) from the opposite team. 

How does this work with computers? The assignment is usually to get through a vulnerability on a server, website, or similar technology asset to get a piece of information that is supposed to be “the flag.” As a quick example, you might need to access `flag.txt`in the root user’s home directory without being the root user or using sudo, with the file or its contents being “the flag.” 

Various types of CTF games cover a broad range of skills in security. For example:

* **Forensics**
    * Recovering data that was not thoroughly deleted or was logged to a different location.
* **Cryptography**
    * Decrypting encrypted data.
* **Web Exploitation**
    * Using common exploits like SQL injection or cross site scripting.
* **Reverse Engineering**
    * Converting compiled code into a human readable format.
* **Binary Exploitation**
    * Using common exploits like buffer overflow or heap overflow.

The goal of playing these games is to bridge the gap between “I understand this in theory” and “I understand this in application.” Thinking more like an attacker leads to more secure code and infrastructure, as you will be able to understand which attacks are more or less likely as well as how successful they are likely to be.


## Establish Trust: Don’t Do “Gotchas” 

We’ve all seen examples in the news of extraordinarily bad phishing tests done by companies to test their staff that range from humorous to hurtful. The intention is usually to use a socially engineered method that will tempt people to click on these emails similar to the way that attackers do. The result is often that people will open the emails and perhaps even click the links, but when they realize they’ve been internally duped, there’s a loss of trust between them and the security team that is trying to tell staff they’re there to help.

Instead of tricking staff, educate staff. If certain types of socially engineered attacks are common—like preying on people’s financial, housing, or other vulnerabilities—teach them what those methods are and show them examples in your training sessions. By both showing what to recognize and being approachable, the security team is able to better improve the business’s security posture. 

For emphasis:

> When staff **trusts** the security team, they are more likely to approach that team when something **does** happen. 

Here at PagerDuty, we have a ***<u>policy not to trick staff, ever</u>***. Common security exploits and methods, including socially engineered attacks, are included in our security trainings. Due to the trust that security has garnered in our organization, staff feel more comfortable approaching security whenever they do discover that they clicked a link from a phishing email or something similar. When things like that happen, security asks clarifying questions, runs a scan on their machine, lets them know of any indicators of compromised security, and then discusses those with them in an accessible way, so the person knows what to do next, if anything. Due to the high degree of trust in our organization, our security team has actually been able to automate a lot around staff reports of security risks, like phishing emails, that were found and reported.

## Socially Engineer Security Trainings

Many of us have needed to sit through pre-recorded security trainings with the goal of improving our ability to navigate common traps in our digital world. That said, many people struggle with these training methods. It’s not uncommon for people to watch them while doing things in the background, or let them play in the background and answer the quiz at the end (if there is one). 

Instead, make your security training engaging. Present about common phishing techniques by showing them—as well as other exploits—but also do things that help engage attendees to keep the content interesting and interactive. In our past security trainings, we’ve shown examples of common passwords exploits in action (demo’ed), as well as “MFA or Not MFA” questions that are instructive for people not familiar with multi-factor authentication. For example:

> MFA or Not MFA: Is it MFA when you answer a security question after entering your password?

Building custom trainings can take a lot of time, but it also allows you to provide more information in areas where your organization is weaker, and be less specific in areas where your organization is stronger. To get started, take a look at our [Security Training Ops Guide](https://sudo.pagerduty.com/)—we have all of our public slides available for all the trainings on that page, as well as their Keynote files and PDF export. Our training materials are open source under the [Apache License](https://github.com/PagerDuty/security-training), so please feel free to use and repurpose to suit the needs of your organization.
