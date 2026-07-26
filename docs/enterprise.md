# ACP Enterprise Program

## Overview

The **ACP Enterprise Program** provides organizations with commercial-grade
support, service-level commitments, and dedicated engagement channels for
adopting and operating the Agentic Commerce Protocol at scale. It is designed
for businesses running ACP in production environments where uptime, response
times, and direct access to maintainers are mission-critical.

The Enterprise Program is a **commercial support tier**, not a governance tier.
Participation does not confer TSC seats, voting rights, or any preferential
treatment in the specification review process. ACP remains an open standard
governed by contribution and consensus, as described in the
[Governance Model](./governance.md).

---

## Why an Enterprise Tier?

ACP is open and free to implement. However, organizations that depend on ACP
for high-volume commerce flows often need more than the community channels
provide — guaranteed response times, a named technical contact, early visibility
into breaking changes, and a clear escalation path when something goes wrong.
The Enterprise Program exists to meet those needs without compromising the
openness or neutrality of the standard itself.

---

## Enterprise Features

### Dedicated Support

- A named **Enterprise Liaison** who serves as your primary point of contact
  within the ACP maintainer team.
- Direct access to a private enterprise support channel alongside the public
  Discord and GitHub channels.
- Priority triage on issues filed against your organization's implementations.

### Service-Level Agreements (SLAs)

| Severity | Description                                | Response Time | Update Cadence |
| -------- | ------------------------------------------ | ------------- | -------------- |
| P1       | Production outage or transaction failure  | 1 business hour | Every 2 hours until resolved |
| P2       | Significant degradation or data issue     | 4 business hours | Daily |
| P3       | Feature question or non-blocking issue     | 2 business days | Weekly |

SLAs apply to issues affecting your organization's use of the published,
stable specification. They do not apply to unreleased drafts, custom forks, or
issues originating outside the ACP specification.

### Early Visibility and Change Management

- Advance notice of breaking changes scheduled for the next spec release, with
  a minimum 30-day window before the change lands in a dated version.
- Access to a quarterly **Enterprise Briefing** covering the roadmap, upcoming
  SEPs, and deprecation schedules.
- Input channel for prioritizing documentation, tooling, and testing resources
  — without bypassing the SEP process for specification changes.

### Implementation Guidance

- Architecture review sessions with ACP maintainers for new integrations.
- Access to a library of reference deployment patterns and conformance test
  suites.
- Onboarding workshops for teams adopting ACP for the first time.

### Recognition

- Organization logo featured on the ACP homepage under an **Enterprise
  Supporters** section, distinct from TSC member logos.
- Permission to reference participation in the ACP Enterprise Program in
  external materials, subject to the guidelines in the
  [Code of Conduct](../CODE_OF_CONDUCT.md).

---

## Engagement Model

### Enrollment

Organizations enroll in the Enterprise Program through a commercial agreement
with the Founding Maintainers (OpenAI and Stripe). The agreement defines the
term, the covered services, and the designated technical contacts within the
customer organization.

### Tiers

The Enterprise Program offers two engagement levels:

| Tier       | Target Audience                          | Liaison Time       | Briefings         |
| ---------- | ---------------------------------------- | ------------------ | ----------------- |
| **Standard** | Single-team or mid-market deployments | Shared, business hours | Quarterly |
| **Premier**  | Multi-team or high-volume deployments | Dedicated, priority response | Monthly + ad-hoc |

Both tiers include the full SLA matrix above; the difference is the depth of
engagement and the cadence of strategic briefings.

### Relationship to Governance

The Enterprise Program is administered by the Founding Maintainers as a
commercial offering. It is explicitly separate from TSC governance:

- Enterprise status does **not** grant a TSC seat or DWG seat.
- Enterprise status does **not** grant voting rights, sponsorship privileges,
  or any authority over the SEP process.
- Enterprise customers propose changes through the same
  [SEP process](./sep-guidelines.md) as any other contributor.
- No enterprise customer receives preferential treatment in how proposals are
  evaluated or adopted. The [Shared Principles](./governance.md#shared-principles)
  apply equally to all participants.

This separation is intentional. The credibility of ACP depends on the standard
evolving through open contribution and consensus — not through commercial
influence. The Enterprise Program funds the ongoing stewardship, tooling, and
support of the protocol, but it does not purchase direction.

---

## Frequently Asked Questions

**Q: Does buying an Enterprise subscription help my organization get a TSC seat?**

A: No. TSC seats are awarded based on contributions and commitment, as described
in the [Governance Model](./governance.md#membership-criteria). Enterprise
status and TSC membership are independent paths. An Enterprise customer that
wishes to join the TSC must earn a seat through the same contribution-based
process as everyone else.

**Q: Can Enterprise customers get breaking changes delayed or exempted for their implementation?**

A: No. The specification evolves through the SEP process for the benefit of the
entire ecosystem. Enterprise customers receive early notice and implementation
support to manage transitions, but they are not exempted from the standard.

**Q: Who provides the support — OpenAI, Stripe, or both?**

A: The Founding Maintainers jointly administer the Enterprise Program. The
specific support model is defined in the commercial agreement and may involve
either or both organizations depending on the customer's integration.

**Q: Is the Enterprise Program required to use ACP in production?**

A: No. ACP is open and free to implement. Many organizations run ACP in
production relying solely on the public documentation, examples, and community
channels. The Enterprise Program is for organizations that want guaranteed
support commitments and deeper engagement.

**Q: How does the Enterprise Program affect the open-source community?**

A: Revenue from the Enterprise Program supports the maintainers' time, tooling,
conformance testing, and documentation that benefit the entire community. The
public channels, examples, and specification remain fully open to all.
