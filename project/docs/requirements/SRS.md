# Software Requirements Specification

**Version:** 1.0  
**Status:** Draft  
**Project:** JeevaFlux  
**Problem Statement:** SIH26181

## 1. Purpose

Define functional and non-functional requirements for the JeevaFlux software
ecosystem supporting on-device health monitoring, risk assessment, early
warnings, mobile interaction and optional secure synchronization.

## 2. Scope

- Sensor data acquisition
- Preprocessing and quality checks
- Feature extraction
- Sensor fusion
- Lightweight local inference
- Personalized baseline
- Risk assessment
- Alert generation
- Mobile companion
- Offline storage
- Optional secure synchronization

## 3. Out of Scope

- Autonomous medical diagnosis
- Replacement of clinical care
- Guaranteed emergency prevention
- Production clinical claims without validation

## 4. System Architecture

See [System Architecture](../architecture/SYSTEM_ARCHITECTURE.md).

## 5. Functional Requirements

See [Functional Requirements](FUNCTIONAL_REQUIREMENTS.md).

## 6. Non-Functional Requirements

See [Non-Functional Requirements](NON_FUNCTIONAL_REQUIREMENTS.md).

## 7. Data Model

See [Data Model](DATA_MODEL.md).

## 8. Safety & Validation

The system must be evaluated for sensor quality, false alerts, missed events,
latency, power consumption, offline behavior and user understanding before
deployment claims are made.
