# OctoAcme — Cross-Functional Collaboration

## Purpose
Define how OctoAcme personas interact with one another, where hand-offs occur, and how to prevent knowledge gaps and ownership ambiguity across the project lifecycle.

---

## Collaboration Principles
- **Explicit hand-offs**: each transition between personas is documented with a clear artifact or acceptance signal.
- **Single source of truth**: decisions and requirements live in the project repository; personas point to it rather than maintaining separate copies.
- **Shared ceremonies**: key personas participate in the relevant parts of planning, review, and retrospective ceremonies.
- **Escalation first**: when ownership is unclear, the Project Manager is the default coordinator until ownership is assigned.

---

## Persona Interaction Map

| Initiating Persona | Collaborates With | Hand-off Artifact / Signal |
|---|---|---|
| Business Analyst | Product Manager | Finalized user stories with acceptance criteria added to backlog |
| Business Analyst | Developer | Requirement walkthroughs and clarification sessions before sprint start |
| Business Analyst | Technical Writer | Approved requirements document as input for documentation drafts |
| UX Designer | Product Manager | Design brief aligned to product goals before wireframing |
| UX Designer | Developer | Design specifications and annotated mockups in the design tool |
| UX Designer | QA/Testing | Visual and interaction acceptance criteria included in the story |
| Developer | DevOps Engineer | Merge to main triggers CI/CD pipeline; environment variables and secrets agreed beforehand |
| Developer | Security Lead | Security-sensitive PRs tagged for Security Lead review |
| Developer | Technical Writer | Feature demo or handoff notes at sprint review for documentation |
| DevOps Engineer | Security Lead | Pipeline security scanning results and access control reviews |
| DevOps Engineer | QA/Testing | Stable test environment provisioned before QA begins |
| Security Lead | Project Manager | Security risk items added to the Risk Register with owner and mitigation |
| Customer Support Representative | Product Manager | Weekly support trend summary with top issues and user pain points |
| Customer Support Representative | Technical Writer | Documentation gap list based on recurring user questions |
| Customer Support Representative | Project Manager | Escalation ticket for critical bugs with user impact data |
| Technical Writer | Developer | Documentation review request before release; developer confirms technical accuracy |
| Technical Writer | Product Manager | Documentation scope and release alignment |

---

## Key Hand-off Points by Lifecycle Phase

### 1. Initiation
- **Business Analyst → Product Manager**: initial requirements brief and stakeholder interview summary
- **Security Lead → Project Manager**: early security and compliance flags added to project charter

### 2. Planning
- **Business Analyst → Developer + QA**: refined user stories with acceptance criteria ready for sprint commitment
- **UX Designer → Developer**: design assets and specifications ready before implementation begins
- **DevOps Engineer → Team**: environment and infrastructure plan shared; deployment constraints identified

### 3. Execution
- **Developer → DevOps Engineer**: code merged to trigger automated pipeline; deployment readiness confirmed
- **Developer → Security Lead**: security-tagged PRs reviewed and approved before merge
- **UX Designer → QA/Testing**: design acceptance criteria used as basis for UI test cases
- **Business Analyst → Developer**: mid-sprint requirement clarifications documented and tracked

### 4. Release
- **DevOps Engineer → Project Manager**: deployment window confirmed; rollback plan in place
- **Technical Writer → Product Manager**: release notes and documentation published before or alongside release
- **Customer Support Representative → Project Manager**: support team briefed on changes and known issues

### 5. Post-Release & Retrospective
- **Customer Support Representative → Product Manager**: post-release feedback summary within one week
- **Security Lead → Team**: security incident or near-miss review included in retrospective
- **Technical Writer → Team**: documentation gaps identified during release captured as backlog items

---

## Standing Meeting Participation Guide

| Ceremony | Required Personas | Optional / As-Needed |
|---|---|---|
| Sprint Planning | PM, PdM, Developer, QA, Business Analyst | UX Designer, DevOps Engineer |
| Daily Standup | Developer, QA | UX Designer, DevOps Engineer, Business Analyst |
| Design Review | UX Designer, Developer, PdM | Business Analyst, QA |
| Security Review | Security Lead, Developer, DevOps Engineer | PM |
| Sprint Demo / Review | PM, PdM, Developer, QA, UX Designer | Business Analyst, Customer Support Representative, Technical Writer |
| Retrospective | PM, PdM, Developer, QA | All personas encouraged |
| Weekly Delivery Sync | PM, PdM | Security Lead, DevOps Engineer, Customer Support Representative |

---

## Resolving Cross-Functional Conflicts

When two personas have conflicting requirements or priorities:

1. **Document the conflict** in the project issue tracker with context from both perspectives.
2. **Bring it to the weekly delivery sync** with the relevant personas present.
3. **Project Manager facilitates** a decision using the principles: customer-first, then risk reduction, then velocity.
4. **Record the decision** in the project decision log so it can be referenced later.

If resolution requires executive input, the Project Manager escalates to the Product Lead or Sponsor per the standard escalation path in [octoacme-risks-and-communication.md](./octoacme-risks-and-communication.md).
