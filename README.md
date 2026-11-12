# DDTS Portfolio Management

## Discovery status

This project is in business discovery. This README records the context, problems, and intended outcomes discussed so far. It is not an agreed set of requirements or an approved operating model.

Discovery baseline updated: 12 November 2026. Findings are based on the sponsor's experience and account; practices outside their area require wider validation. References to GDS and ITIL describe reported departmental practice, not an independent assessment of compliance with external guidance.

The project is currently a personal initiative sponsored by the repository owner, intended to be presented to senior leaders later. The Chief Digital and Information Officer (CDIO) is a potential future sponsor, not a confirmed sponsor. Changes to processes and governance may be proposed; adoption will be decided later.

## Business context

See the [current process flow](docs/current-process.md) for a visual account of demand, shaping, mobilisation, delivery, live services, and annual funding, including known gaps and validation points.

Individual diagrams are available in [As Is Discovery](As%20Is%20Discovery):

- [Demand and shaping](As%20Is%20Discovery/01-demand-and-shaping.md)
- [Mobilisation, delivery, and live services](As%20Is%20Discovery/02-mobilisation-delivery-and-live-services.md)
- [Annual funding and financial oversight](As%20Is%20Discovery/03-annual-funding-and-financial-oversight.md)

The focus is Defra's Digital, Data, Technology and Security (DDTS) area. DDTS has no single view of all the work it needs to do, its importance, who is doing it, or its position in lifecycle stages and governance steps.

Demand ranges from small, newly conceived ideas to mature policy initiatives that have had no digital input. Work is managed through smaller portfolios within delivery groups and through other routes, including Service Transformation.

## Working problem statement

DDTS lacks a shared view of demand and work across its lifecycle, alongside clear boundaries for delivery responsibility and decision-making. Demand is handled through separate portfolios and delivery routes, with inconsistent approaches to shaping, prioritisation, capacity planning, business approval, and technical governance.

This contributes to duplicated effort, work falling between teams, delayed mobilisation and decisions, and pressure on supplier contract headroom. Importance is currently driven by the availability of funding, without an explicit link between work and strategic outcomes.

## Discovery findings

### Demand and engagement

- Demand reaches DDTS through several channels. Some delivery groups are engaged early through formal business relationships, but most requests arrive through ad hoc emails.
- A published engagement form has low uptake. Feedback is limited, but customers have reported not knowing which delivery group to approach.
- The sponsor's delivery group records engagements as tickets on a Jira board. Other groups use different approaches, including spreadsheets and SharePoint lists.
- The sponsor's group investigates every engagement it receives. This has not been established as the practice across all groups.
- In one example, a project started and the delivery team subsequently discovered that two other teams were investigating the same problem.

### Shaping and progression

- In the sponsor's delivery group, a shaping team develops an initiative request proposal covering the problem statement, risks, assumptions, and related information.
- Business sign-off of that proposal normally precedes supplier engagement or resource allocation. Other delivery groups follow different processes.
- Early shaping time is not charged to the business, although it consumes internal capacity.
- Shaping is often paused while the business seeks approvals or decisions. Requests may remain open or be moved to a blocked column on the local Jira board.
- Delivery groups handle readiness and progression differently; no consistent DDTS-wide approach has been established in this discovery.

### Prioritisation and strategic alignment

- Importance is currently determined by who has funding.
- Work is not currently linked back to strategic outcomes.
- Delivery group leads, service design leads, strategy leads, and principal architects need to look across the full portfolio to identify overlapping and competing demand.
- Defra has an internally published strategic outcome framework that is not yet public. Its content has not been reviewed as part of this discovery.
- Many initiatives can be mapped to that framework, but the sponsor has encountered work with no clear mapping. The reason for these gaps has not yet been established.

### Capacity and supplier commitments

- Capacity visibility is limited and is generally managed within individual professions.
- The sponsor's area uses a SharePoint list to track resources assigned to projects. Capacity planning approaches in other areas are not yet known.
- Capacity is provided through permanent staff, resource augmentation, outcome supplier contracts, and specialist contracts for niche work.
- Teams shape the problem and identify the team or resource needed, but capacity is not usually considered until project mobilisation.
- Resource augmentation has a reported lead time of six to eight weeks, which can delay mobilisation.
- More work has been started under outcome supplier contracts than forecast, increasing burn rates and leaving no contract headroom.
- Capacity discovery therefore needs to consider both people and skills availability and supplier delivery commitments and contractual headroom.
- Profession leads are responsible for capacity within their professions; supplier management is responsible for capacity in its respective area.
- Capacity is normally secured separately from funding and governance approvals.

### Business ownership and decisions

- Ownership of the business outcome is often unclear.
- Business engagement is commonly delegated to a mid-tier member of staff, with occasional senior engagement.
- Work can stall while the business representative seeks approval from the business owner or resolves debate about costs and whether the appropriate business governance has taken place.
- Delegation itself is not established as the problem; the authority and accountability accompanying it need further exploration.

### Cross-portfolio decision-making

- Leads can make decisions within their own delivery group. The sponsor's stated authority boundary is that they should escalate potential overlap and should not decide matters affecting multiple delivery groups or Service Transformation individually.
- Delivery groups sit under the Chief Product Officer (CPO); Service Transformation sits under the Chief Digital Officer (CDO).
- There is no established group above the delivery groups for cross-portfolio decisions and no existing escalation route other than to the CPO and CDO.
- An issue might subsequently be discussed at executive board, but the sponsor is not aware of this happening.

### Governance and technical assurance

- Digital governance and business-area governance can overlap and duplicate activity.
- Teams can be uncertain about which approvals are required and whether they have been completed.
- Across Service Transformation and delivery groups, responsibility for technical assurance and sign-off of implementations is unclear.
- Business ownership of a service, DDTS responsibility for its technology and delivery, and authority to approve technical changes are distinct matters that need clarification.
- The sponsor, a principal architect, has attempted to provide technical assurance for Service Transformation work affecting their area, with limited success.

### Lifecycle, approvals, and transition to live

The four main lifecycle stages reported are **Demand, Mobilisation, Delivery, and Live services**. Shaping takes place within Demand.

- Delivery includes substages following the GDS agile delivery lifecycle. A project delivery lifecycle is being phased out as agile adoption increases. A procurement lifecycle is also used where an agile approach is unsuitable for the initiative.
- During shaping, the business representative normally confirms that funding has been agreed. This generally means an allocation for the current financial year, not assured funding for the whole initiative.
- DDTS would prefer to contribute digital input before the business writes its outline business case. Business case sign-off is normally expected; its precise timing and evidence across routes remain to be validated.
- **Approval to spend** authorises expenditure on Digital and Data work and is required before Mobilisation. It is provided by **PAB, the Portfolio Assurance Board**.
- Technical assurance takes place through service assessments following GDS guidance. Architectural governance occurs at Alpha and Beta, during Delivery.
- The Chief Technology Officer participates in PAB and can challenge technical concerns.
- Service Transformation normally does not follow the same approval route because the group funds its own work. How architectural approval and technical risk acceptance are handled remains unclear.
- Before production deployment, work must go through the **Service Design Review Board**. Live services normally becomes involved during Delivery, in private beta.
- Live services reviews project work and allocates resources for activities including knowledge articles, help desk onboarding, and whole-life cost modelling.
- Live services follows ITIL. Limited understanding of ITIL among delivery staff has caused difficulties.
- The department is seeking to move towards a "you build it, you run it" operating model, but the sponsor reports limited success so far.
- Ongoing support, including bug fixes and keeping services running, is usually defined. Continuous improvement arrangements are not normally agreed.

### Blocked, withdrawn, and completed work

- Delivery groups normally review blocked engagements locally. Review frequency has not been established.
- The business representative normally has authority to withdraw an engagement. The sponsor has not seen DDTS walk away from one; DDTS's formal authority or criteria for doing so remain unknown.
- Beyond maintaining their own SharePoint list, the sponsor has not seen routine updates to capacity commitments and portfolio records when work pauses, is cancelled, or completes. Practice elsewhere needs validation; this is not evidence that no updates occur anywhere in DDTS.

### Funding, spend, and forecasting

- Businesses bid for further funding each financial year. Suppliers sometimes continue working at risk while continued funding is negotiated; the authorisation and contractual arrangements for this have not been established.
- Most initiatives reportedly secure continued funding until the minimum viable product (MVP) is delivered, after which funding moves to service support. Continuous improvement funding is not normally settled.
- The sponsor knows of some approved-budget spreadsheets but does not know the authoritative source or owner of approved-budget information.
- Actual spend for permanent staff and resource augmentation is maintained in the ERP system. Monthly purchase orders are raised to pay supplier invoices and recorded in the ERP.
- Spend is normally linked to an initiative, with possible roll-up to programme level.
- Supplier management maintains forecasts largely as projected burn-down of contract headroom, with limited intelligence from planned work informing them.
- Programme delivery managers typically maintain delivery forecasts in spreadsheets.
- Whether contract and programme forecasts reconcile, and how they relate to approved budgets, remains unknown.

## Delivery landscape

### Delivery groups

The delivery groups identified during discovery are:

- Nature Recovery
- Flood
- Environmental Quality
- Animal and Plant Health
- Farming
- Planning Reforms
- Trade and EU
- Waste and Circular Economy
- Group Corporate Services

Some groups are effectively large programmes, while others align directly with business areas. There are no clear bounded contexts between the groups, contributing to both gaps in responsibility and duplicated work.

### Service Transformation

There is no specified definition of when work should go to a delivery group versus Service Transformation.

Service Transformation offers two main service provisions:

- Fast-paced discovery to understand a specific business problem.
- Light-touch process optimisation, often using process automation or robotics.

It also has workstreams focused on Grants, Licences and Permits, and Customer, which are not yet fully defined.

Service Transformation may work with the same customers as delivery groups, without those groups having visibility. It draws on the same professions but uses different contracts to provide capacity.

This has caused confusion over technical assurance and sign-off, particularly when Service Transformation changes services that normally fall within a delivery group's remit. A portfolio view limited to delivery groups would therefore omit a relevant delivery route.

## Intended outcomes

The sponsor has identified three primary outcomes:

1. **Clearer visibility of the whole portfolio:** Cover demand and work at all lifecycle stages across delivery groups and Service Transformation, including importance, responsibility, lifecycle position, and governance progress.
2. **Better management of capacity:** Improve understanding of delivery commitments and capacity across professions and sourcing routes, including mobilisation lead times and supplier contract headroom.
3. **Better linkage to strategic outcomes:** Make the relationship between work and strategic outcomes visible and support more informed prioritisation.

**Stretch outcome:** Better visibility of actual spend against approved spend. Feasibility and scope have not yet been assessed.

## Sponsor's proposed changes and planning principles

These are proposals for later consideration, not adopted DDTS policy or approved requirements:

- Provide visibility of all DDTS work, irrespective of size, across all lifecycle stages and delivery routes.
- Establish an agreed route and authority for resolving cross-boundary issues. A particular forum or organisational structure has not been selected.
- Make the business sponsor the definitive voice on how an initiative contributes to strategic outcomes.
- Distinguish strategic change, live services, technical risk, and statutory obligations as reasons for work. Statutory work may also contribute to strategic outcomes; justification and strategic contribution can coexist. Final classification rules remain open.
- Allow DDTS to reject initiatives that cannot demonstrate a strategic contribution or another agreed justification. Decision authority, criteria, and escalation arrangements would need agreement.
- At Demand stage, plan by role type rather than named individuals, with visibility of supplier capacity and contract headroom.
- Use a capacity planning horizon of at least six months. Supplier availability and contractual headroom are separate considerations.

## Success criteria and measurement status

| Primary outcome | Sponsor's definition of success | Measurement still needed |
| --- | --- | --- |
| Whole-portfolio visibility | Account for the totality of DDTS work, irrespective of size. | Define what constitutes a work item and how coverage, completeness, and currency will be checked across delivery routes. |
| Capacity management | Initially, fewer surprises about contract headroom; as permanent staffing grows, earlier identification of role and skill shortages. | Establish current headroom surprises, forecast accuracy, and notice periods for shortages before setting targets. |
| Strategic alignment | Work demonstrates contribution to strategic outcomes or another agreed justification; DDTS can reject initiatives without either. | Establish current mapping and justification coverage, validation responsibilities, and decision authority before setting targets. |

Actual versus approved spend remains a stretch outcome. No quantitative baselines or targets have been agreed. The measurement topics above are candidates for validation, not committed metrics.

## Remaining uncertainties and validation needs

The initial open discovery questions have been explored with the sponsor. The following points still need evidence, wider validation, or a decision:

- Confirm recording, shaping, prioritisation, capacity planning, and progression practices across other delivery groups and Service Transformation.
- Identify the full set of delivery routes and work sources needed to establish complete DDTS coverage, including small work and live service activity.
- Agree authority for cross-portfolio decisions and escalation, including decisions to reject, combine, redirect, sequence, pause, or stop work.
- Review the internal strategic outcome framework with authorised stakeholders and understand why some work does not map to it.
- Clarify business outcome accountability, delegated authority, technology responsibility, architectural approval, and technical risk acceptance, particularly for Service Transformation.
- Validate lifecycle variants, business case approval timing, governance evidence, and the boundaries between business and digital governance.
- Clarify responsibility and funding for continuous improvement, and the intended operating model after go-live.
- Establish how paused, blocked, inactive, withdrawn, cancelled, and completed work is reviewed and how commitments are updated.
- Understand the effect of stalled work on allocated people and supplier commitments beyond early shaping.
- Identify authoritative approved-budget information and reconcile initiative, programme, contract, ERP, and forecast records.
- Understand the authorisation and commercial arrangements when suppliers continue working before further funding is confirmed.
- Establish baselines and realistic measures for the primary outcomes before agreeing targets.

## Next discovery step

Use this README as the discovery baseline for validation with relevant stakeholders before defining requirements. No product features, technology choices, common governance model, or changes to organisational responsibilities have been agreed. Improvements to visibility will need supporting decisions about accountability, governance, and maintaining reliable information.
