# Non-Functional Requirements

## Performance

- Core local monitoring should be low-latency.
- Exact latency targets must be established by benchmarking on the selected
  hardware.
- Memory and compute budgets should be defined for each edge model.

## Power

- Sampling and inference schedules should be optimized for extended operation.
- Battery performance must be measured under representative workloads.

## Reliability

- Core monitoring should not require continuous internet connectivity.
- The system should recover gracefully from sensor dropout and reconnection.

## Security

- Authenticated access.
- Encrypted network transport.
- Secure credential/token handling.
- Least-privilege access.
- Auditability for sensitive operations.

## Privacy

- Local processing wherever practical.
- Data minimization.
- Consent-based optional sharing.
- Defined retention/deletion behavior.

## Usability

- Alerts must be understandable at a glance.
- Avoid unnecessary repeated notifications.
- Support accessible, regional-language-ready interfaces.

## Scalability

The architecture should permit additional risk models, sensors, users and
authorized analytics without redesigning the core data pipeline.
