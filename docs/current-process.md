# DDTS current process flow

Based on sponsor-led discovery as at 12 November 2026. This is a description for validation, not an approved process or a future-state design. The delivery group detail primarily reflects the sponsor's group; other groups vary.

Solid arrows show the reported progression. Dotted lines show context, exceptions, or relationships whose detailed process is not established. A decision box does not imply that a formal, consistently enforced gate exists.

## Demand and shaping

```mermaid
flowchart TD
    A["Business demand: early idea through to mature policy initiative"] --> B["Engagement through relationships, ad hoc emails, or low-use form"]
    B --> C["Demand reaches a delivery group or Service Transformation"]
    C -.-> GAP["No defined routing boundary; overlap and gaps may remain unseen"]
    C --> DG["Delivery group: record locally in Jira, spreadsheet, or SharePoint"]
    C --> ST["Service Transformation: internally funded route"]
    DG --> SH["Shaping team investigates and prepares initiative request proposal: problem, risks, assumptions"]
    SH --> F["Business representative confirms current financial-year funding"]
    F --> SIGN{"Business sign-off and required business decisions secured?"}
    SIGN -->|Not yet| BLOCK["Pause shaping; request remains open or blocked; delivery group reviews"]
    BLOCK --> SEEK["Business representative seeks owner approval, cost decisions, or governance clearance"]
    SEEK --> SIGN
    BLOCK -.-> WITH["Business representative may withdraw engagement"]
    SIGN -->|Yes| PAB["PAB: approval to spend required before mobilisation; CTO can challenge technical concerns"]
    PAB -->|Approval granted| MOB["Proceed to mobilisation"]
    ST --> STR["Rapid discovery or light-touch process optimisation; other workstreams still being defined"]
    STR -.-> STG["Normally outside delivery group approval route; technical approval and risk acceptance unclear"]
    DG -.-> ESC["Cross-boundary issue: escalate to CPO and/or CDO; no established resolution forum"]
    ST -.-> ESC
```

Business case approval is normally expected, but its exact timing across routes is unconfirmed. Early DDTS involvement before the outline business case is a preference, not an established universal step. PAB refusal, deferral, and resubmission arrangements have not been described.

## Mobilisation, delivery, and live services

```mermaid
flowchart TD
    M["Mobilisation following PAB approval to spend"] --> CAP["Secure capacity separately; availability usually considered at mobilisation"]
    CAP --> SOURCE["Permanent staff, resource augmentation, outcome supplier contract, or specialist contract"]
    SOURCE -.-> OWN["Profession leads and supplier management manage respective capacity"]
    SOURCE -.-> DELAY["Resource augmentation: 6-8 week lead time; supplier contract headroom can constrain delivery"]
    SOURCE --> D["Delivery using appropriate lifecycle"]
    D --> AG["GDS agile delivery substages"]
    D --> OTHER["Project lifecycle being phased out; procurement lifecycle used where appropriate"]
    AG -.-> ARCH["Architectural governance at Alpha and Beta"]
    AG -.-> ASSURE["Service assessments provide assurance"]
    AG --> PB["Private beta: live services normally becomes involved"]
    PB --> SDRB["Service Design Review Board before production deployment"]
    OTHER -.-> SDRB
    ST["Service Transformation implementation, where applicable"] -.-> SDRB
    SDRB --> PREP["Live service preparation: knowledge articles, help desk onboarding, whole-life cost modelling"]
    PREP --> PROD["Production deployment and live services"]
    PROD --> SUPPORT["Support, bug fixes, and keeping the service running usually defined"]
    PROD -.-> CI["Continuous improvement ownership and funding normally not agreed"]
    PROD -.-> MODEL["ITIL live service processes; move towards 'you build it, you run it' remains unsettled"]
```

The Service Design Review Board was described as required before go-live. The precise Service Transformation handoff and the mapping of non-agile routes to that review need validation; dotted connectors do not assert a confirmed sequence. Review outcomes, formal acceptance criteria, and the exact sequencing of preparation activities have not been detailed.

## Annual funding and financial oversight

This runs alongside the lifecycle, rather than being a single stage in it.

```mermaid
flowchart TD
    FY["Business has current financial-year allocation"] --> WORK["Initiative progresses"]
    WORK --> NEXT["Bid for funding for the next financial year"]
    NEXT --> STATUS{"Continued funding confirmed?"}
    STATUS -->|Pending| RISK["Suppliers sometimes continue working at risk while funding is negotiated"]
    RISK -.-> NEXT
    STATUS -->|Yes| CONT["Continue delivery; most initiatives reportedly funded through MVP"]
    CONT --> MVP["MVP delivered"]
    MVP --> SUP["Funding moves to service support; improvement funding often unresolved"]
    WORK -.-> ERP["Actual staff and augmentation spend plus supplier purchase orders recorded in ERP"]
    WORK -.-> FC["Programme delivery managers maintain spreadsheet forecasts"]
    WORK -.-> CONTRACT["Supplier management forecasts contract headroom burn-down"]
    ERP -.-> GAP["Approved-budget source and reconciliation between financial views not established"]
    FC -.-> GAP
    CONTRACT -.-> GAP
```

The process when continued funding is refused has not been established. Working at risk is a reported practice, not a recommendation or confirmation of commercial authorisation.

## Main gaps exposed by the flow

- No consistent routing or shared check for overlapping demand across delivery groups and Service Transformation.
- Cross-boundary decision authority and escalation are not formalised below CPO/CDO level.
- Business authority, funding decisions, and governance can leave shaping blocked.
- Capacity and contract headroom are considered late and separately from approvals.
- Service Transformation technical approval and risk acceptance are unclear.
- Live service engagement normally begins in private beta; continuous improvement responsibility and funding remain unsettled.
- Blocked and closed work does not have a visibly consistent process for updating portfolio and capacity commitments.
- Strategic alignment and rejection of unjustified demand are proposed changes, not steps in the current flow.

See the [discovery baseline](../README.md) for evidence, proposed changes, success criteria, and remaining questions.
