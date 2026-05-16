# Audit Scope & Organisational Context
**Document:** GRC-DOC-001
**Version:** 1.1
**Date last revised:** 16 May 2026
**Author:** N.Haitham
**Review:** Self-reviewed (portfolio project)

## 1. Purpose

This document establishes the scope, boundaries, and organisational context for the TechNova Ltd GRC audit. It is the foundation document from which all subsequent workpapers are derived. Getting this right upfront is critical, because a poorly defined scope is probably the single biggest reason why ISMS implementations struggle.

## 2. Organisational Context (Relating to ISO 27001 Clause 4)

### 2.1 Understanding the Organisation

TechNova Ltd is a cloud-native B2B SaaS business. Their core product is a project management platform used by SMEs and a small number of UK public sector clients. The business is venture-backed and is growing fast, which means security controls have historically been heavily reactive rather than proactive or planned.

**Key internal factors:**
- Rapid headcount growth (40% YoY), onboarding and offboarding processes are immature, and not well established
- Engineering-heavy culture; security seen as a blocker by some teams, rather than something that is crucial
- No dedicated CISO; CTO owns security alongside engineering responsibilities, leading to security sometimes falling behind/ being neglected
- Recent SOC 2 Type I passed (external), although some foundational controls exist
- AWS infrastructure managed by a 4-person platform/DevOps team

**Key external factors:**
- GDPR obligations (processes UK and EEA personal data)
- Contractual security requirements from public sector clients (NHS framework, G-Cloud)
- Growing client security questionnaire burden (roughly 3 to 4 per month)
- Cyber insurance renewal requires evidence of control improvements
- Competitive pressure: ISO 27001 certification increasingly expected at procurement

### 2.2 Interested Parties

| Party | Interest / Requirement |
|-------|----------------------|
| Clients (SME) | Data confidentiality, uptime, GDPR compliance |
| Public sector clients | ISO 27001, Cyber Essentials+, DSPT alignment |
| Investors (Series A) | Risk management maturity, due diligence readiness |
| Cyber insurer | Evidence of controls; MFA, patching, BCP |
| ICO (regulator) | GDPR compliance, breach notification capability |
| AWS (cloud provider) | Shared responsibility model adherence |
| Employees | Clear security policies, training, acceptable use |
| Board | Governance, risk oversight, reputational risk |

## 3. ISMS Scope Statement (ISO 27001 Clause 4.3)

> *The ISMS covers the design, development, hosting, and support of the TechNova project management platform, including the AWS cloud infrastructure (EU west 2 and EU central 1 regions), Manchester headquarters, and remote-working employees in the UK and Poland. The scope includes all information assets used to deliver the platform and support client operations.*
### 3.1 In-Scope Assets

- AWS cloud environment (EC2, RDS, S3, VPC, IAM, CloudTrail, GuardDuty)
- Platform source code and CI/CD pipelines (GitHub, GitHub Actions)
- Client data (project data, user PII, usage analytics)
- Corporate IT systems (M365, Slack, Jira, Confluence, Okta SSO)
- Physical: Manchester HQ (open plan, server room cabinet, visitor access)
- Employees and contractors with access to in-scope systems
