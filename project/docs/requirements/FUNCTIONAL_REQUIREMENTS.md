# Functional Requirements

| ID | Requirement | Priority |
|---|---|---|
| JF-FR-01 | Acquire configured physiological sensor measurements | High |
| JF-FR-02 | Acquire configured environmental measurements | High |
| JF-FR-03 | Timestamp incoming readings | High |
| JF-FR-04 | Detect missing/invalid/noisy readings | High |
| JF-FR-05 | Perform local preprocessing | High |
| JF-FR-06 | Extract windowed features | High |
| JF-FR-07 | Fuse multimodal signals | High |
| JF-FR-08 | Maintain a personal baseline | High |
| JF-FR-09 | Estimate supported risk states | High |
| JF-FR-10 | Generate graded alerts | High |
| JF-FR-11 | Display status and warnings in mobile app | High |
| JF-FR-12 | Store selected records locally | High |
| JF-FR-13 | Continue core warning functions offline | High |
| JF-FR-14 | Synchronize permitted records after reconnection | Medium |
| JF-FR-15 | Show historical trends/events | Medium |
| JF-FR-16 | Show device/connectivity/battery status | Medium |
| JF-FR-17 | Record alert acknowledgement | Medium |
| JF-FR-18 | Enforce consent before optional sharing | High |

## Risk Modules

Each module should expose:

- Input signals
- Data-quality conditions
- Feature set
- Risk logic/model
- Confidence/uncertainty
- Alert severity
- Recommended user action
- Validation dataset/scenario
