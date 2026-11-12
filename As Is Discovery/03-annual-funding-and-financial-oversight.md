# Annual funding and financial oversight

Based on sponsor-led discovery as at 12 November 2026. Current process for validation, not an approved operating model. Delivery group details primarily reflect the sponsor's group; other groups vary.

Solid arrows show reported progression. Dotted lines show context, exceptions, or relationships whose detailed process is not established. Decision boxes do not imply consistently enforced gates.

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

[Discovery baseline](../README.md) | [All process flows](../docs/current-process.md)

