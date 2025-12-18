# Dynamic Device-Centric Trust Tokens for IoMT (DTT-RBAC)

This repository supports research on **Dynamic Device-Centric Trust Tokens (DTT)** for
real-time **Role-Based Access Control (RBAC)** in **Internet of Medical Things (IoMT)**
networks.

## Motivation
IoMT deployments rely heavily on static credentials and long-lived role assignments.
Such static trust models fail to capture the dynamic operational state of medical devices,
allowing malfunctioning or compromised devices to retain privileged access.
This project explores a lightweight, zero-trust-inspired approach where devices must
continuously prove their trustworthiness before exercising assigned roles.

## Core Idea
Each IoMT device periodically generates a short-lived cryptographic trust token that
binds:
- device identity
- assigned RBAC role
- real-time device health indicators (e.g., firmware integrity, battery level, latency)

A gateway verifies these tokens and enforces access control decisions based on both
the device's role and its current operational health.

## Scope
This repository is currently focused on:
- system design and threat modeling
- literature review and gap analysis
- experimental planning and evaluation metrics

Implementation artifacts will be added incrementally as the research progresses.

## Research Status
- [x] Problem formulation
- [x] Research gaps identified
- [x] System design finalized
- [ ] Device-side token generation
- [ ] Gateway verification and RBAC enforcement
- [ ] Experimental evaluation

## References
This work builds on prior research in IoMT security, IoT access control, and device
attestation, including but not limited to:
- IoMT security surveys
- IoT RBAC and access control frameworks
- Remote attestation mechanisms for constrained devices

## License
This project is licensed under the MIT License.


