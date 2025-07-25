# Helm Security Process and Policy

This document provides the details on the Helm security policy and details the processes
surrounding security handling including a how to guide on reporting a security vulnerability
for anything within the Helm organization.

## Report A Vulnerability

We’re extremely grateful for security researchers and users who report vulnerabilities
to the Helm community. All reports are thoroughly investigated by a set of Helm maintainers.

To make a report please email the private security list at cncf-helm-security@lists.cncf.io
with the details.

You may, but are not required to, encrypt your email to this list using the PGP keys
of security team members, listed below.

| Name           | Key URL                                                                                         | Fingerprint                                        |
|----------------|-------------------------------------------------------------------------------------------------|----------------------------------------------------|
| Andrew Block   | [link](https://keybase.io/sabre1041/pgp_keys.asc)                                               | 2CE5 F1FB 9E8C 59B8 7BBD  5F2B 02DF E631 AEF3 5EBC |
| George Jenkins | [link](https://keybase.io/gjenkins8/pgp_keys.asc)                                               | C048 04B5 F250 1D25 CA69  A415 2945 4FC9 6455 D41E |
| Matt Butcher   | [link](https://keybase.io/technosophos/pgp_keys.asc)                                            | ABA2 5295 98F6 626C 420D 335B 62F4 9E74 7D91 1B60  |
| Matt Farina    | [link](https://keybase.io/mattfarina/pgp_keys.asc)                                              | 672C 657B E06B 4B30 969C 4A57 4614 49C2 5E36 B98E  |
| Robert Sirchia | [link](https://keys.openpgp.org/vks/v1/by-fingerprint/7FEC81FACC7FFB2A010ADD13C2D40F4D8196E874) | 7FEC81FACC7FFB2A010ADD13C2D40F4D8196E874           |

### When To Send A Report

You think you have found a vulnerability in a Helm project or a dependency of a Helm project. This can be any of the repositories on the [Helm GitHub organization](https://github.com/helm).

### When Not To Send A Report

* If a vulnerability has been found in an application deployed by a Helm Chart. Instead, contact the application maintainers
* For guidance on securing Helm, please see the [documentation](https://helm.sh/docs/using_helm/#securing-your-helm-installation) or ask in one of the [support channels](README.md#how-can-i-help)
* You are looking for help applying security updates

### Security Vulnerability Response

Each report will be reviewed and receipt acknowledged within 3 business days. This will set off the security review process detailed below.

Any vulnerability information shared with the security team stays within the Helm project and will not be shared with others unless it is necessary to fix the issue. Information is shared only on a need to know basis.

We ask that vulnerability reporter(s) act in good faith by not disclosing the issue to others. And we strive to act in good faith by acting swiftly, and by justly crediting the vulnerability reporter(s) in writing.

As the security issue moves through triage, identification, and release the reporter of the security vulnerability will be notified. Additional questions about the vulnerability may also be asked of the reporter.

### Public Disclosure

A public disclosure of security vulnerabilities is released alongside release updates or details that fix the vulnerability. We try to fully disclose vulnerabilities once a mitigation strategy is available. Our goal is to perform a release and public disclosure quickly and in a timetable that works well for users. For example, a release may be ready on a Friday but for the sake of users may be delayed to a Monday.

CVEs will be assigned to vulnerabilities. Due to the process and time it takes to obtain a CVE ID, disclosures will happen first. Once the disclosure is public the process will begin to obtain a CVE ID. Once the ID has been assigned the disclosure will be updated.

If the vulnerability reporter would like their name and details shared as part of the disclosure process we are happy to. We will ask permission and for the way the reporter would like to be identified. We appreciate vulnerability reports and would like to credit reporters if they would like the credit.

## Security Team Membership

The security team is made up of a subset of the Helm project maintainers who are willing and able to respond to vulnerability reports.

### Responsibilities

* Members MUST be active project maintainers on active (non-deprecated) Helm projects as defined in [the governance](governance/governance.md)
* Members SHOULD engage in each reported vulnerability, at a minimum to make sure it is being handled
* Members MUST keep the vulnerability details private and only share on a need to know basis

### Membership

New members are required to be active maintainers of Helm projects who are willing to perform the responsibilities outlined above. The security team is a subset of the maintainers. Members can step down at any time and may join at any time.

From time to time, Helm projects are deprecated. If at any time a security team member is found to be no longer be an active maintainer on active Helm projects, this individual will be removed from the security team.

## Patch and Release Team

When a vulnerability comes in and is acknowledged, a team - including maintainers of the Helm project affected - will assembled to patch the vulnerability, release an update, and publish the vulnerability disclosure. This may expand beyond the security team as needed but will stay within the pool of Helm project maintainers.

## Disclosures

Vulnerability disclosures are published as blog posts on the [Helm Blog](https://helm.sh/blog/) and emailed to the [Helm mailing list](https://lists.cncf.io/g/cncf-helm). The disclosures will contain an overview, details about the vulnerability, a fix for the vulnerability that will typically be an update, and optionally a workaround if one is available.

Disclosures will be published on the same day as a release fixing the vulnerability after the release is published.
