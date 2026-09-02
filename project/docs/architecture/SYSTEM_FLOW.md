# JeevaFlux System Flow

```mermaid
flowchart TD
    A[Sensor Acquisition] --> B[Signal Processing]
    B --> C[Sensor Fusion]
    C --> D[On-Device TinyML / Risk Inference]
    D --> E[Personal Baseline + Context]
    E --> F[Risk Score / Risk State]
    F --> G{Risk Threshold}
    G -->|Normal| H[Continue Monitoring]
    G -->|Caution / High Risk| I[User Alert + Guidance]
    G -->|Emergency Candidate| J[Escalation Workflow]
    H --> K[Local Event / Trend Storage]
    I --> K
    J --> K
    K --> L{Connectivity?}
    L -->|Yes| M[Secure Synchronization]
    L -->|No| N[Store Locally]
    N --> L
```

## Processing Sequence

1. Acquire measurements.
2. Check signal quality.
3. Preprocess and extract features.
4. Fuse physiological, environmental and contextual signals.
5. Compare against personal baseline.
6. Estimate risk.
7. Generate a graded warning when appropriate.
8. Store the event locally.
9. Synchronize permitted records when connectivity returns.
