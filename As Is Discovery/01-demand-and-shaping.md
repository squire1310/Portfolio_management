# Demand and shaping

Based on sponsor-led discovery as at 12 November 2026. Current process for validation, not an approved operating model. Delivery group details primarily reflect the sponsor's group; other groups vary.

Solid arrows show reported progression. Dotted lines show context, exceptions, or relationships whose detailed process is not established. Decision boxes do not imply consistently enforced gates.

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

[Discovery baseline](../README.md) | [All process flows](../docs/current-process.md)

