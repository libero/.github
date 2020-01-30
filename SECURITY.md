# Vulnerabilities in Libero Software
There are a number of modules that make up the various products in the Libero Suite. These are each represented under individual repositories for modules and related configuration or scripts. They also depend on a large set of third party libraries (e.g., react.js, koa, express). It is possible that a module or its dependent libraries contain vulnerabilities that would allow triggering unexpected or dangerous behavior with specially crafted inputs.

## What is a vulnerability?
Given Libero is built to be user-facing and take input, it is possible to specify inputs which exhibit unexpected or unwanted behaviour. While we have independent third-parties perform security testing intermittently, and review changes to the software with known security threats in mind, it may be possible to cause issues especially where the software reads and writes files, communicates via the network, accesses databases or executes code that could cause infinite loops, or run out of memory. It is only when these behaviours are outside the specifications of the operations involved that such behaviour is a vulnerability.

As a general rule, it is incorrect behaviour for any Libero software to access memory it does not own, or to terminate in an unclean way. Bugs in Libero software that lead to such behaviors constitute a vulnerability.

# Reporting vulnerabilities
Please email reports about any security related issues you find to [security@libero.pub](mailto:security@libero.pub). This mail is delivered to a small security team. Your email will be acknowledged within one business day, and you'll receive a more detailed response to your email within 7 days indicating the next steps in handling your report.

Please use a descriptive subject line for your report email. After the initial reply to your report, the security team will endeavour to keep you informed of the progress being made towards a fix and announcement.

In addition, please include the following information along with your report:

- Your name and affiliation (if any).
- A description of the technical details of the vulnerabilities. It is very important to let us know how we can reproduce your findings.
- An explanation who can exploit this vulnerability, and what they gain when doing so -- write an attack scenario. This will help us evaluate your report quickly, especially if the issue is complex.
- Whether this vulnerability is public or known to third parties. If it is, please provide details.
- If you believe that an existing (public) issue is security-related, please send an email to [security@libero.pub](security@libero.pub). The email should include the issue ID and a short description of why it should be handled according to this security policy.

Once an issue is reported, the Libero Team use the following disclosure process:

- When a report is received, we confirm the issue and determine its severity.
- If we know of specific third-party services or software based on Libero software that require mitigation before publication, those projects and teams will be notified.
- An advisory is prepared (but not published) which details the problem and steps for mitigation.
Wherever possible, fixes are prepared for the last minor release of the two latest major releases, as well as the master branch. We will attempt to commit these fixes as soon as possible, and as close together as possible.
- Patch releases are published for all fixed released versions, a notification is sent to the [#general channel in the Libero Community Slack](https://libero.pub/join-slack/), and the advisory is published.

Past security advisories are listed below. We credit reporters for identifying security issues, although we keep your name confidential if you request it.

# Security Advisories
None to date.


# Credit
Adapted from https://github.com/tensorflow/tensorflow/blob/master/SECURITY.md