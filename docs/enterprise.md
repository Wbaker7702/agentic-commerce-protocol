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

### Security and Compliance

- **Security advisories** delivered ahead of public disclosure, with a private
  channel for triaging vulnerabilities affecting your integration.
- Annual **security review** of your ACP integration surface, covering
  authentication flows, payment handler boundaries, and data exposure paths.
- Compliance mapping documents for PCI DSS, SOC 2, and GDPR, describing how ACP
  protocol boundaries map to common control frameworks. These are reference
  materials, not legal attestations.
- Coordinated disclosure timeline: enterprise customers receive a minimum
  14-day advance notice of security-relevant spec changes before public release.

### Conformance Certification

Enterprise customers may pursue **ACP Conformance Certification** for their
implementations. Certification is a voluntary attestation that an implementation
passes the full ACP conformance test suite for a given dated spec version.

- Access to the **certification test harness** with automated and guided test
  scenarios covering agentic checkout, delegate payment, delegate authentication,
  and cart flows.
- A named **Certification Engineer** who runs the test suite against your
  implementation and produces a conformance report.
- A versioned **Certificate of Conformance** valid for the dated spec version
  tested, renewable when you upgrade to a new dated version.
- Listing on the ACP homepage under a **Certified Implementations** registry,
  with the spec version and certification date.

Certification is a verification of protocol conformance, not an endorsement of
the implementation's business practices or reliability. The ACP maintainers
may revoke a certificate if the implementation is found to materially diverge
from the tested version.

### Multi-Region and High-Availability Guidance

- Reference architectures for multi-region ACP deployments, including patterns
  for payment handler failover, cart state replication, and idempotency across
  regions.
- Guidance on regional data residency considerations for delegate payment and
  delegate authentication flows, mapping protocol boundaries to common
  regulatory regions (EU, US, India, Brazil, and others as adopted).
- Load testing templates and suggested SLOs for high-volume checkout paths,
  calibrated against the reference implementation's observed performance.

### Technical Account Manager (Premier Tier)

Premier-tier customers are assigned a **Technical Account Manager (TAM)** in
addition to the Enterprise Liaison. The TAM:

- Runs a monthly **service review** covering open issues, SLA performance, and
  upcoming spec changes relevant to your integration.
- Maintains a living **integration runbook** documenting your organization's
  ACP surface area, dependencies, and upgrade path.
- Coordinates cross-team escalations when an issue spans multiple ACP areas
  (for example, a change that affects both cart and delegate payment).
- Acts as a stable technical contact across personnel changes on the customer
  side, reducing onboarding friction when new engineers join the integration.

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

Both tiers include the full SLA matrix above. The difference is the depth of
engagement, the cadence of strategic briefings, and access to a dedicated
Technical Account Manager (Premier only). The full feature comparison is
below.

### Feature Comparison

| Feature                                      | Standard | Premier |
| -------------------------------------------- | :------: | :-----: |
| Named Enterprise Liaison                     |    ✓     |    ✓    |
| Private enterprise support channel           |    ✓     |    ✓    |
| Priority issue triage                        |    ✓     |    ✓    |
| Full SLA matrix (P1/P2/P3)                   |    ✓     |    ✓    |
| Early visibility on breaking changes         |    ✓     |    ✓    |
| Architecture review sessions                 |    ✓     |    ✓    |
| Security advisories and annual security review |   ✓    |    ✓    |
| Compliance mapping documents                 |   ✓     |    ✓    |
| Conformance Certification access            |    ✓     |    ✓    |
| Multi-region reference architectures         |   ✓     |    ✓    |
| Enterprise Briefings                         | Quarterly | Monthly + ad-hoc |
| Dedicated Technical Account Manager          |          |    ✓    |
| Monthly service review                       |          |    ✓    |
| Living integration runbook                    |          |    ✓    |
| Cross-team escalation coordination           |          |    ✓    |
| Liaison availability                         | Business hours | Priority response |

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

## Onboarding Playbook

New enterprise customers follow a structured onboarding path to reach steady-state
support. The timeline is indicative; the Enterprise Liaison adjusts it to the
customer's integration maturity.

1. **Week 1 — Kickoff.** Introduction to the Enterprise Liaison (and TAM, if
   Premier). Confirm covered services, designated technical contacts, and
   support channel access. Review the commercial agreement scope.
2. **Week 2 — Integration Review.** Architecture review session covering the
   customer's current or planned ACP surface area: which spec areas are in use,
   which payment handlers are involved, and where cart and checkout flows
   integrate.
3. **Week 3 — Security and Compliance Walkthrough.** Walk through the security
   advisory channel, the coordinated disclosure timeline, and the compliance
   mapping documents relevant to the customer's regulatory regions.
4. **Week 4 — Conformance and Testing.** Introduce the certification test
   harness. For customers pursuing certification, schedule the first test run
   with the Certification Engineer.
5. **Ongoing — Steady State.** The customer enters normal SLA coverage. Premier
   customers begin the monthly service review cadence with the TAM. All
   customers receive the next scheduled Enterprise Briefing.

Customers may accelerate or compress this timeline for time-sensitive
launches. The Enterprise Liaison works with the customer to adjust.

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

**Q: What is the difference between the Enterprise Liaison and the Technical Account Manager?**

A: The Enterprise Liaison is the primary support contact for all enterprise
customers and handles issue triage and SLA coordination. The Technical Account
Manager (Premier tier only) takes a deeper, ongoing role: running monthly
service reviews, maintaining the integration runbook, and coordinating
escalations that span multiple ACP areas. The TAM is a stable technical contact
across personnel changes on the customer side.

**Q: Is Conformance Certification required to deploy ACP in production?**

A: No. Certification is a voluntary attestation that an implementation passes
the full conformance test suite for a given spec version. Many organizations
deploy ACP without it. Certification is useful when you need a verifiable
statement of conformance for partners, auditors, or internal governance.

**Q: Do the compliance mapping documents make my integration PCI DSS or SOC 2 compliant?**

A: No. The compliance mapping documents describe how ACP protocol boundaries
map to common control frameworks. They are reference materials to support your
own compliance work, not legal attestations. Your organization remains
responsible for its own compliance posture.
