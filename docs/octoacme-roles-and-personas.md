# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

---

## UX Designer

### Role Summary
UX Designers create intuitive, accessible, and visually consistent user experiences. They bridge the gap between user needs and technical implementation by delivering wireframes, prototypes, and validated design assets.

### Responsibilities
- Conduct user research and usability testing to inform design decisions
- Produce wireframes, mockups, and interactive prototypes
- Define and maintain design systems and style guides
- Review implemented UIs to ensure they match design specifications
- Advocate for accessibility and inclusive design standards

### Goals
- Deliver interfaces that are easy to use and visually consistent
- Reduce friction and support errors in user-facing flows
- Ensure design decisions are grounded in user research and data

### Typical Communication
- Design reviews with Product Managers and Developers before sprint start
- Prototype walkthroughs with QA and stakeholders for acceptance sign-off
- Async feedback via design tools (e.g., Figma comments) and PR reviews for UI changes

### Interactions with Existing Personas
- **Product Manager**: aligns design scope with product goals and prioritization
- **Developer**: collaborates on feasibility, handoff specs, and implementation review
- **QA/Testing**: provides acceptance criteria for visual and interaction quality
- **Business Analyst**: uses requirements and user stories to shape design flows

---

## DevOps Engineer

### Role Summary
DevOps Engineers automate build, test, and deployment pipelines and manage the infrastructure that supports development, staging, and production environments. They ensure reliable, repeatable, and secure delivery processes.

### Responsibilities
- Design and maintain CI/CD pipelines for automated testing and deployment
- Provision and manage cloud infrastructure and environment configurations
- Monitor system health, performance, and availability
- Implement and enforce security controls in the delivery pipeline
- Support incident response and postmortem processes for infrastructure issues

### Goals
- Minimize deployment risk through automation and repeatability
- Ensure high availability and fast recovery from failures
- Shift security and quality checks left in the delivery pipeline

### Typical Communication
- Sprint planning participation to assess infrastructure work items
- On-call rotation and incident response channels
- Pull request reviews for infrastructure-as-code and pipeline changes

### Interactions with Existing Personas
- **Developer**: provides tooling, environments, and deployment guidance
- **QA/Testing**: ensures test environments mirror production and CI runs all checks
- **Security Lead**: implements security scanning and access controls in pipelines
- **Project Manager**: communicates deployment windows, downtime risks, and environment readiness

---

## Business Analyst

### Role Summary
Business Analysts bridge the gap between stakeholder needs and engineering execution. They gather, document, and validate requirements and translate them into actionable work items with clear acceptance criteria.

### Responsibilities
- Elicit and document functional and non-functional requirements through stakeholder interviews and workshops
- Write user stories, process flows, and acceptance criteria for backlog items
- Facilitate requirement reviews with stakeholders and the delivery team
- Identify gaps, conflicts, and ambiguities in requirements before work begins
- Track requirement coverage and sign-off throughout the project lifecycle

### Goals
- Ensure the delivery team always works from clear, agreed-upon requirements
- Reduce mid-sprint scope changes caused by misunderstood needs
- Maintain a traceable link between business goals and delivered features

### Typical Communication
- Requirement walkthroughs and story-refinement sessions with Project Manager and Developers
- Stakeholder sign-off meetings before sprint commitment
- Documentation updates in the project wiki or knowledge base

### Interactions with Existing Personas
- **Project Manager**: aligns requirements to timeline and milestone planning
- **Product Manager**: translates product vision into detailed acceptance criteria
- **Developer**: clarifies requirements during refinement and development
- **Technical Writer**: shares finalized requirements for documentation drafting

---

## Technical Writer

### Role Summary
Technical Writers produce clear, accurate, and maintainable documentation for internal teams and external users. They capture institutional knowledge and ensure it is accessible and kept up to date.

### Responsibilities
- Write and maintain user guides, API references, runbooks, and process documents
- Collaborate with Developers and Product Managers to document new features at release time
- Establish and enforce documentation standards and templates
- Review and improve existing documentation for clarity and accuracy
- Manage the documentation release process in sync with product releases

### Goals
- Ensure every feature and process has clear, findable documentation
- Reduce support burden by producing self-service resources for users
- Preserve institutional knowledge and reduce onboarding time for new team members

### Typical Communication
- Participation in sprint reviews and feature demos to capture documentation needs
- Review cycles with Developers and Product Managers before publishing
- Async collaboration via pull requests and doc comments

### Interactions with Existing Personas
- **Developer**: reviews code and implementation notes to write accurate technical content
- **Product Manager**: aligns documentation scope with release priorities
- **Business Analyst**: uses finalized requirements as input for documentation drafts
- **Customer Support Representative**: incorporates common user questions into FAQs and guides

---

## Security Lead

### Role Summary
The Security Lead defines and enforces security standards, conducts threat modeling, and coordinates the organization's response to security incidents. They embed security practices across all phases of the project lifecycle.

### Responsibilities
- Define and maintain the organization's security policies, standards, and guidelines
- Conduct threat modeling and security reviews for new features and architecture changes
- Oversee security scanning in CI/CD pipelines and triage findings
- Lead incident response and coordinate post-incident retrospectives
- Ensure compliance with relevant regulatory and industry standards

### Goals
- Prevent security vulnerabilities from reaching production
- Minimize the blast radius and recovery time of security incidents
- Build a culture of security awareness across all teams

### Typical Communication
- Security review sessions during design and pre-release phases
- Incident response bridges and post-incident reports
- Async review of PRs and architecture documents with security implications

### Interactions with Existing Personas
- **DevOps Engineer**: implements security controls and scanning in pipelines
- **Developer**: provides secure coding guidance and reviews security-sensitive code changes
- **Project Manager**: flags security risks and compliance requirements during planning
- **Product Manager**: advises on security trade-offs for product decisions

---

## Customer Support Representative

### Role Summary
Customer Support Representatives are the front line of user interaction. They capture user pain points, common issues, and feedback trends and channel this intelligence back to the product and engineering teams to guide prioritization.

### Responsibilities
- Respond to user inquiries and resolve support tickets in a timely manner
- Identify recurring issues, bugs, and friction points from support data
- Escalate critical bugs or outages to the Project Manager and engineering team
- Participate in release reviews to flag potential support impacts
- Contribute user feedback and pain points to the product backlog

### Goals
- Deliver a positive user experience through fast, accurate support
- Reduce ticket volume by influencing product improvements and documentation
- Serve as the voice of the user in planning and prioritization discussions

### Typical Communication
- Weekly support trend summaries shared with Product Manager and Project Manager
- Escalation channels for critical bugs and outages
- Participation in sprint reviews and retrospectives to share user perspective

### Interactions with Existing Personas
- **Product Manager**: provides quantitative and qualitative user feedback to inform roadmap
- **Project Manager**: escalates critical issues that require immediate engineering attention
- **Technical Writer**: highlights documentation gaps based on common user questions
- **Developer**: reports reproducible bugs with steps to reproduce and user context

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

