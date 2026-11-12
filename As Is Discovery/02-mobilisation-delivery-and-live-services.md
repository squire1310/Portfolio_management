# Mobilisation, delivery, and live services

Based on sponsor-led discovery as at 12 November 2026. Current process for validation, not an approved operating model. Delivery group details primarily reflect the sponsor's group; other groups vary.

Solid arrows show reported progression. Dotted lines show context, exceptions, or relationships whose detailed process is not established. Decision boxes do not imply consistently enforced gates.

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

[Discovery baseline](../README.md) | [All process flows](../docs/current-process.md)

