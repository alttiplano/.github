# Security

At **Alttiplano**, we take the security of our open-source tools, developer platforms, and products very seriously. We appreciate the researchers and community members who help us keep our software secure.

This is the default security policy for all Alttiplano repositories. If a repository has its own `SECURITY.md`, that one takes precedence.

## ⚠️ Important

**We do not accept unverified automated scanner dumps or AI-generated security reports.** We receive a large number of hallucinated or non-actionable reports and do not have the resources to review them all.

- Reports without a valid, reproducible Proof of Concept (PoC) demonstrating a security impact may be closed without further investigation.
- Repeated spam submissions may result in a ban from the Alttiplano organization.

AI-assisted security research is welcome, provided a human has verified the findings and a working PoC is included.

## Supported Versions

Only the **latest release** and the `main` branch receive security patches. If you are on an older version, please upgrade.

## Threat Model

Alttiplano builds open-source tools, developer platforms, and applications. Many of them run locally on your machine and can inspect, edit, or execute files and commands you provide. Permission prompts and UI warnings exist for user awareness, not as a security sandbox, unless a product explicitly documents one.

### Out of Scope

The following are generally out of scope, unless they demonstrate a distinct, exploitable vulnerability within an Alttiplano product.

| Category                           | Rationale                                                                      |
| ---------------------------------- | ------------------------------------------------------------------------------ |
| **Expected local tool behavior**   | Tools executing user-provided commands or scripts as intended                  |
| **Unauthenticated local services** | Dev servers bound to `localhost` for single-user use                           |
| **Third-party services & APIs**    | Upstream dependencies, external LLM providers, or plugins outside our boundary |
| **Denial of Service (DoS)**        | Resource exhaustion on local desktop software without privilege escalation     |
| **Missing best practices**         | Missing headers or flags that do not lead to an exploitable vulnerability      |

## Reporting Security Issues

Please **do not disclose vulnerabilities publicly** until we have had a chance to review and fix them.

To report an issue, go to the repository under [github.com/alttiplano](https://github.com/alttiplano), open the **Security** tab, and click **Report a vulnerability**. If that option is not available on a repository, or for organization-wide matters, use the email at the bottom of this page.

Please include:

- A clear description of the vulnerability and its impact
- Step-by-step instructions to reproduce it
- The environment, operating system, and software version tested
- Relevant logs or screenshots, if any
- Suggested mitigations or patches, if you have them

We do not currently offer a bug bounty.

## Disclosure

We follow coordinated disclosure and aim to ship a fix within 90 days of acknowledging your report. Once a fix is verified, we will publish a patched release and a GitHub Security Advisory crediting you, unless you prefer to remain anonymous.

## Escalation

We aim to acknowledge every report within 5 business days. If you have not received an acknowledgement by then, send us an email:

📧 **Email:** [`security@alttiplano.com`](mailto:security@alttiplano.com)