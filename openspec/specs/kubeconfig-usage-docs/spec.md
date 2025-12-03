# kubeconfig-usage-docs Specification

## Purpose
TBD - created by archiving change add-kubeconfig-usage-doc. Update Purpose after archive.
## Requirements
### Requirement: Kubeconfig Usage Documentation
The documentation SHALL provide a Sealos-specific kubeconfig usage guide covering retrieval, download, import, and local tooling usage.

#### Scenario: Access paths documented
- **WHEN** users need kubeconfig for Sealos-managed clusters
- **THEN** the guide explains how to obtain and download kubeconfig via Sealos Desktop UI and CLI, including context and namespace scope.

#### Scenario: Local tooling validation
- **WHEN** users follow the guide
- **THEN** they can configure kubeconfig for kubectl, helm, and k9s, and verify connectivity with example commands.

#### Scenario: CI/CD automation
- **WHEN** kubeconfig is used in pipelines (e.g., GitHub Actions)
- **THEN** the documentation provides a minimal-permission workflow example with secret injection guidance and cache considerations.

#### Scenario: App Launchpad integration
- **WHEN** applications are deployed via Sealos App Launchpad
- **THEN** the guide explains how to supply kubeconfig (e.g., secret mounting or context selection) and outlines common deployment or debug operations.

#### Scenario: App Launchpad API automation
- **WHEN** GitHub Actions workflows manage Launchpad apps via the `POST /api/v1/app` API
- **THEN** the documentation shows how to call the API with tokens/secrets, example payloads, and notes on minimal permissions.

#### Scenario: Security and lifecycle guidance
- **WHEN** kubeconfig credentials are issued or rotated
- **THEN** the documentation outlines permission scope, expiry or rotation guidance, and steps to revoke compromised kubeconfigs.

#### Scenario: Troubleshooting support
- **WHEN** connection or authentication issues occur
- **THEN** the guide lists common causes (e.g., certificate expiry, RBAC denial, endpoint reachability) and actionable remediation steps.

#### Scenario: Navigation entry
- **WHEN** users browse primary documentation entry points
- **THEN** the kubeconfig usage guide is discoverable from the main README or documentation index.

