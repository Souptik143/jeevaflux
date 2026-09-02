# Architecture Decision Record

## ADR-001 — Edge-First Intelligence

**Decision:** Keep core time-sensitive monitoring and risk inference local where
hardware constraints permit.

**Reason:** Supports low-latency behavior, privacy and operation during
connectivity loss.

**Trade-off:** Edge hardware has tighter memory, compute and power budgets.

## ADR-002 — Multimodal Sensor Fusion

**Decision:** Combine physiological, environmental and contextual features.

**Reason:** Risk interpretation can depend on environmental exposure and activity,
not just one physiological measurement.

**Trade-off:** Fusion requires more careful data-quality handling and validation.

## ADR-003 — Offline-First Storage

**Decision:** Retain selected events locally and synchronize later.

**Reason:** Disaster and rural environments can have intermittent connectivity.

**Trade-off:** Local storage security and conflict/retry handling must be designed.
