![Terminology](/assets/images/headers/terminology.png)

As you start your DevSecOps journey, it’s important to use common language and share common concepts with your security team. To help you get started, here are some industry terms and concepts, some of which you’ll need in the guide directly, but all of which you’ll need as you broaden your knowledge.

## OWASP and NIST


**<u>OWASP**</u> (Open Web Application Security Project) and **<u>NIST**</u> (National Institute for Standards and Technology, US Based) are two heavily used resources for security tools, resources, and research.

## Security posture

An organization's **<u>security posture**</u> is the overall security status across your technical organization, including software, networking, data, vendor risk, dependency security, vulnerability management, and more. Knowing your security posture is vital to understanding how at risk you are to various types of security threats, such as data breaches, and will allow you to know what to remediate and with what urgency.

## Attack Vector and Attack Surface

An **<u>attack vector**</u> is any method that an intruder can use to gain access to your systems and information. For example, if/when a key is committed to GitHub, if someone else used that key to access the service, that exposed credential would be considered an attack vector. The **<u>attack surface**</u> is all of the attack vectors. For example, the exposed credential, any unencrypted data, and so forth, would be your organization’s attack surface.

## Perimeter

A **<u>perimeter**</u> is the barrier that prevents access, similar to what you would see with physical security where natural or built walls, etc., prevent access. In this case, the walls would be what separates public and private networks, firewalls, access controls, and so forth.

## Security Breach

A **<u>security breach**</u> is whenever someone gains unauthorized access of any kind, including network or application access.

## Data Breach

A **<u>data breach**</u> is any release of confidential information to public sources. Common examples are credit card numbers, government ID numbers, addresses, and other identifying information. The release may be unintentional or intentional. Note the difference between a security breach and a data breach: the security breach is the gaining of access (“breaking in”) and the data breach is taking information out from where it was secured (the “theft”, also referred to as **<u>exfiltration**</u>).

## Exploit

An **<u>exploit**</u> is code that takes advantage of a vulnerability.

## Trust

Establishing **<u>trust**</u> is the verification that a resource or user is who is claimed. An example of a trusted resource might be verifying that the application patch or update is from an intended source, or that the user who is attempting to access data is associated with the intended person or entity.

## Zero Trust

Although there are other models, in recent years **<u>zero trust**</u> is a model for security that has become an industry standard. In fact, we practice it here at PagerDuty. Concisely, zero trust is a model for continuous authorization. It does not assume that, because a user is able to access certain data or devices, that that user should be there, so users are always prompted for their credentials for access. As an example, in a zero trust environment, the network a user is coming from does not grant assumed access, e.g. if the user is connecting via a company VPN—all access requests still need to be authenticated.

## Threat Actor

**<u>Threat actors**</u> are the types of individuals or groups that you anticipate are most likely to try to breach your security measures. For example, you might find that you are most likely to be hit by scripts that are not targeting you directly, but instead are targeting a service that you are using or region you are in.

## Risk Management

**<u>Risk management**</u> is the ongoing process of identifying what security risks you have in your organization and how to prevent, mitigate, and resolve them. It starts by identifying the risk associated with various assets, such as personal information, and determining both how likely they are to be the focus of an attack and what the impact of an attack would be if it were to happen.

## White Hat vs Black Hat

Usually in reference to hacking, a **<u>white hat**</u> hacker is a person who hacks or tests the security of a system with the owner’s permission and informs the owner of all vulnerabilities found. Conversely, a **<u>black hat**</u> hacker is someone who tests the security of a system, usually with the intent to breach it, without the owner’s permission and does not inform them of vulnerabilities found. As an example, a white hat hacker or group might be a security consultancy brought in to run a pen test, whereas a black hat hacker might be trying to steal customer credit card information. As a quick note, you may also come across the term **<u>grey hat**</u>, which is someone who breaches security but without the malicious intent of a black hat attacker.

## White Box vs Black Box

**<u>Black box**</u> is when a system is known only by its behavior, basically its inputs and outputs, without knowing anything about how it is built (e.g. AWS vs GCP). On the other hand, **<u>white box**</u> is when you know the architecture of a system. These terms are usually used in reference to testing, where black box testing is when you test an unknown system and white box testing is testing a known system.

## Red Team, Blue Team, Purple Team

Similar to white hat hackers, **<u>red teams**</u> specialize in breaching security, with permission. Red team exercises are usually done by security teams to simulate what an external attacker is likely to do in order to obtain whatever they are targeting, e.g. secure data. On the opposite side is the **<u>blue team**</u>, which specializes in defensive security. Blue team exercises can be the defensive response to red team exercises, but they can also be other things like audits. When red teams and blue teams coordinate, it’s called **<u>purple teaming**</u>.
