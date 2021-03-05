![Shift Security Left](../assets/img/headers/shift_left.png)

Simply put: shifting security left means integrating security earlier in the SDLC. This is a different approach to how security is currently implemented, where their team is mostly reacting to a current incident, or being consulted as a last-step before something is released to production. Looking at the latter case first for a moment, that means that any insecure code that was designed and implemented has made it through the entire lifecycle before being reviewed. If security finds an issue, that means changes are likely to go back around the full cycle again before going live in production. 

When security issues are found they require not only modifications to the codebase, but also other changes elsewhere in the life cycle (e.g. updating tests, monitoring, etc.). Shifting security left allows teams to address security issues much earlier in the life cycle, rather than finding out after significant labor has already taken place.

Shifting security left is a series of tasks—it is not meant to be something that you implement quickly. Just like all other changes in IT, the best way to proceed is with small changes, reviews, and iterations. You will need to start with a security assessment, perform organizational training and exercises to improve your security posture. For reference, there is also a list of security actions and tests at different phases (or stages) in the SDLC at the end of the section.

## Identify Your Needs With a Security Assessment

Before you can begin shifting left, you need to know your current status. You might think of this as the “security health” of your org, and the industry term for this is your “security posture.” Specifically, security posture is defined as:

 * Security posture refers to an organization's overall cybersecurity strength and how well it can predict, prevent and respond to ever-changing cyberthreats. ([Source](https://searchsecurity.techtarget.com/definition/security-posture))

Why look at your security posture? The main goal is to provide some context for how you should proceed when you shift left. Should you move slowly from right to left across the SDLC, implementing tests and procedures as you go? Should you fix forward and choose a project that starts with security considerations from the design phase? Or should you choose an approach that is a hybrid of the above options?

The answer is that it depends and can vary widely. The best way forward is to “meet yourself where you’re at.” The security assessment will provide information that you can use to determine your next steps. Specifically, the security assessment should inform you of any current security risks and their criticality. Some questions the assessment will need to address:

* Have there been any security incidents? 
* What are your current risks?
* How critical are they?

Once you have this information, the first questions you should discuss with your security team are:

* Which security incidents that are at risk of repeating can be resolved with changes to security procedures?
* What critical risks can be mitigated or resolved by changing security procedures?

Resolving current or likely security incidents should be the first priority as you shift left. After these are addressed, you’ll want to start focusing on ways that you can build momentum and show the value by choosing those courses of action that will be “high value, low lift.” Translated into something more actionable, this means the development, operations, and security teams will need to work together to find which changes in security procedure have a high impact by influencing multiple factors—while minimizing how much customization is required. As you build momentum and the benefit of shifting left is more tangible, you can iterate more changes to improve your overall security posture.

## Assessment Frameworks

How to decide which assessment(s) to run, and executing them, is under the purview of your security team. That said, there are some frameworks that you can take a look at to have a better understanding of what goes into assessments in general to know what roughly to expect. These frameworks can also help establish a starting point for your own assessments, rather than your team customizing one from scratch. Some common frameworks include:

* [DSOMM](https://owasp.org/www-project-devsecops-maturity-model/) (OWASP’s DevSecOps Maturity Model)
* [BSIMM](https://www.bsimm.com/) (Building Security In Maturity Model)
* [SAMM](https://owasp.org/www-project-samm/) (OWASP’s Software Assurance Maturity Model)
* [NIST’s Infrastructure Security Framework](https://nvlpubs.nist.gov/nistpubs/CSWP/NIST.CSWP.04162018.pdf)

If your company is part of a regulated industry, you’ll also want to verify if there are frameworks available that tailor to that industry. For example, Qualys is an approved vendor for PCI compliance and offers a web vulnerability scanner to help organizations become compliant.
