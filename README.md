LOGOS
Public Interface / Protected Core Architecture
LOGOS is an infrastructure-grade Layer 1 system built under a Protected Core architectural model.
This repository provides public integration contracts, observable guarantees, and operational documentation required for technical evaluation and enterprise integration.
The core execution implementation remains proprietary.
Architectural Model
LOGOS follows a strict separation of concerns:
Public Interface Layer
Documented and externally verifiable
Defines integration contracts
Describes observable behavior and guarantees
Protected Core Layer
Proprietary execution logic
Consensus and finality control
Security-critical mechanisms
Internal optimization and protection systems
Public contracts define behavior.
Internal mechanisms define how that behavior is achieved.
Repository Scope
This repository contains:
Architecture principles (behavioral, not algorithmic)
Public API surface (redacted OpenAPI specification)
Threat model (public security posture)
Integration contracts
Sanitized infrastructure templates (non-production)
Security disclosure process
Governance & contribution policy
These materials describe:
Externally observable behavior
Integration expectations
Operational boundaries
Deployment assumptions (abstracted)
Observable Guarantees
Although the core implementation is proprietary, the following properties are externally verifiable:
Deterministic transaction ordering
Atomic block commit semantics
Strict nonce enforcement
Anti-duplication guarantees at the interface boundary
Public REST API contract stability
Defined failure modes
Health and monitoring endpoints
Behavior can be evaluated independently of implementation details.
Out of Scope
This repository does not include:
Core execution engine source code
Consensus or finality algorithms
Internal security parameters
Production infrastructure topology
Real deployment domains or IP addresses
Secrets, tokens, signing infrastructure
Partner-only or administrative endpoints
Any materials not explicitly included should be considered proprietary.
Partner Review Model
Proprietary components may be reviewed under controlled access:
NDA-based documentation access
Controlled audit environments
Read-only technical review under agreement
➡ See: docs/05-partner-nda-process.md
Security Reporting
Please do not disclose vulnerabilities via public issues.
Use:
GitHub Private Vulnerability Reporting
Process defined in SECURITY.md
Responsible disclosure policy applies.
Licensing
This repository provides documentation and integration materials only.
It does not grant open-source rights to the LOGOS core implementation.
See LICENSE for applicable terms.
Status
Core execution layer: operational (proprietary)
Public interface: stabilizing
Enterprise integrations: controlled access
