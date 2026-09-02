# System Architecture

## Architecture Overview

JeevaFlux can be represented as a layered architecture:

```mermaid
flowchart TB
    subgraph S["Sensing Layer"]
        P1[Heart Rate]
        P2[SpO2]
        P3[Skin Temperature]
        P4[Motion / Activity]
        P5[Sleep / Recovery]
        P6[GSR]
        E1[Temperature]
        E2[Humidity]
        E3[PM2.5 / PM10 / AQ]
    end

    subgraph I["Edge Intelligence"]
        Q[Signal Quality]
        X[Preprocessing]
        F[Feature Extraction]
        M[Multimodal Fusion]
        AI[Lightweight AI / Risk Inference]
    end

    subgraph R["Risk & Action"]
        B[Personal Baseline]
        RS[Risk State]
        AL[Alert Engine]
    end

    subgraph U["User Layer"]
        APP[Mobile Companion]
        HIST[History & Trends]
    end

    subgraph C["Optional Synchronization"]
        L[Local Storage]
        SY[Secure Sync]
        CL[Authorized Backend / Analytics]
    end

    S --> Q --> X --> F --> M --> AI
    AI --> B --> RS --> AL --> APP
    APP --> HIST
    X --> L
    L --> SY --> CL
```

## Layer Responsibilities

| Layer | Responsibility |
|---|---|
| Sensing | Acquire physiological and environmental measurements |
| Signal Quality | Identify missing/unreliable/noisy measurements |
| Processing | Filtering, normalization and feature generation |
| Fusion | Combine complementary signals and context |
| AI | Lightweight local inference / anomaly and risk assessment |
| Personalization | Compare with user-specific baseline |
| Alerts | Convert risk into understandable action-oriented notifications |
| Mobile | User interaction, trends, status and history |
| Local Storage | Offline event retention |
| Sync | Optional secure synchronization after reconnection |

## Design Principle

The architecture separates **time-critical local functions** from optional
cloud functions. This supports the project's offline-first and privacy-first
goals.
