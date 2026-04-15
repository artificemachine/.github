# Security Policy

Artifice Machine takes the security of its tools, protocols, and configurations seriously. This policy describes how to report vulnerabilities and what to expect in response.

## Reporting a Vulnerability

**Please do not report security vulnerabilities through public GitHub issues, discussions, or pull requests.**

Instead, report them through one of the following private channels:

### Preferred: GitHub Private Vulnerability Reporting

For repositories in this organization that have it enabled, use GitHub's built-in private vulnerability reporting:

1. Navigate to the affected repository
2. Click the **Security** tab
3. Click **Report a vulnerability**
4. Fill in the details

This is the fastest path because it creates a private discussion attached to the affected code.

### Alternative: Email

Send a detailed report to:

**security@artificemachine.com**

Please include:

- A clear description of the vulnerability
- The affected repository, version, and component
- Steps to reproduce
- Potential impact (data exposure, code execution, denial of service, etc.)
- Any suggested mitigation, if you have one
- Whether you would like public credit for the discovery

If your report contains sensitive details, you may encrypt it. A PGP key fingerprint will be published here once available.

## What to Expect

### Acknowledgement

We will acknowledge receipt of your report within **3 business days**. Given that Artifice Machine is a small workshop, this may sometimes be longer for reports received during travel or maintenance windows.

### Triage

Within **7 business days** of acknowledgement, we will:

- Confirm whether the issue is a vulnerability we can reproduce
- Assess severity using a CVSS-like framework
- Provide an initial estimate of remediation timeline
- Identify whether other repositories or downstream users are affected

### Remediation

Severity-dependent timelines for fixes:

| Severity | Target fix window |
|---|---|
| Critical (active exploitation, broad data exposure) | 7 days |
| High (privilege escalation, significant data exposure) | 30 days |
| Medium (limited exposure, requires non-default config) | 60 days |
| Low (minor information disclosure, requires unusual setup) | 90 days |

These are targets, not guarantees. We are honest about delays when they occur.

### Disclosure

We follow **coordinated disclosure**:

- A fix is prepared and reviewed privately
- The fix is released to users
- A public advisory is published 7 days later (longer for severe issues with active exploitation)
- Reporters who want public credit are credited in the advisory

If a vulnerability is being actively exploited in the wild, we may shorten this timeline.

## Scope

This policy covers all repositories under `github.com/artificemachine`. It does not cover:

- Vulnerabilities in upstream dependencies (please report those upstream first; we will respond to advisories that affect us)
- Issues that are not security vulnerabilities (use the public issue tracker for those)
- Vulnerabilities in personal repositories at `github.com/newblacc` or `github.com/celstnblacc` (those are separate; report directly to the operator)

## Safe Harbor

We will not pursue legal action against researchers who:

- Make a good-faith effort to comply with this policy
- Avoid privacy violations, data destruction, or service disruption during testing
- Do not exploit the vulnerability beyond what is necessary to confirm it
- Report through the channels listed above before public disclosure
- Give us a reasonable opportunity to fix the issue before going public

We appreciate responsible research and will work with you in good faith.

## Out of Scope

The following are not considered vulnerabilities for the purposes of this policy:

- Missing security headers without a demonstrated impact
- Vulnerabilities in third-party services we use but do not operate
- Social engineering attacks against the operator or users
- Physical attacks
- Denial-of-service attacks against rate-limited public services
- Reports generated solely by automated scanners without human verification

## Hall of Thanks

Researchers who have responsibly disclosed vulnerabilities are credited here, with their permission:

*(none yet)*

---

*Last updated: 2026-04-15*
*Operated by: Artifice Machine, a brand of NewBlacc.*
