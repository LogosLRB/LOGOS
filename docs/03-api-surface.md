Public API Surface
Interface Boundary Definition
This document defines the supported public API surface of LOGOS.
Only endpoints explicitly documented in this specification are considered part of the supported public integration contract.
Endpoints not listed in this document should be treated as internal and not subject to public compatibility guarantees.
1. Public API Categories
The public API surface is divided into the following categories.
1.1 Core Query Endpoints
These endpoints expose externally observable finalized state:
/healthz
/head
/balance/{rid}
These endpoints are read-only and return information derived from publicly visible finalized state.
1.2 Transaction Submission Endpoints
/submit_tx
This endpoint allows submission of transactions subject to documented validation rules.
Transaction acceptance does not imply inclusion in finalized state.
Finalization status must be determined via documented public state query endpoints.
2. Public Contract Properties
The public API contract provides:
Deterministic response structures under documented operating conditions
Structured and documented error responses
Versioned contract stability for endpoints classified as Stable
Explicit success and failure indicators
No exposure of internal execution details or protected mechanisms
The API contract applies exclusively to documented public endpoints.
3. Stability Levels
Public API endpoints are classified as follows.
Stable
Covered by semantic versioning principles
Breaking changes require a major version increment
Backward-compatible changes maintain contract continuity
Experimental
May change without a major version increment
Clearly marked in the OpenAPI specification
Not covered by long-term compatibility expectations
Only endpoints explicitly marked as Stable are covered by compatibility guarantees.
4. Explicitly Excluded Surfaces
The following categories are not part of the public API surface:
Administrative endpoints
Debug or diagnostic endpoints
Partner-only or restricted endpoints
Bridge or settlement endpoints
Metrics endpoints (unless explicitly documented as public)
Internal service-to-service interfaces
These interfaces are internal and not covered by public compatibility guarantees.
5. Versioning Model
The public API follows semantic versioning principles:
MAJOR — breaking changes
MINOR — backward-compatible feature additions
PATCH — backward-compatible fixes
Version identifiers are machine-detectable via documented public endpoints.
6. Interface Boundary
This document defines the public contract boundary.
Internal mechanisms, validation thresholds, control parameters, execution logic, and deployment characteristics remain outside the public API surface.
Integrations should rely solely on documented public endpoints and published contract guarantees.
7. Change Governance
Changes to the public API surface require:
Documentation update
OpenAPI specification update
Version increment where applicable
Maintainer approval
Endpoints not explicitly documented should not be relied upon for integration.
