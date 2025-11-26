# Security Overview

Security posture of **DevSecOps Pipeline Security**.

## Shift-Left Security

- **SAST**: Static code analysis
- **SCA**: Dependency vulnerability scanning
- **Secrets detection**: Pre-commit hooks
- **IaC scanning**: Terraform/CloudFormation checks

## Pipeline Security

- **IAM least privilege**: Per-stage roles
- **Artifact signing**: Code provenance
- **Encrypted secrets**: Secrets Manager
- **Audit logging**: All pipeline actions

## Container Security

- **Image scanning**: ECR + Inspector
- **Base image policies**: Approved images only
- **Runtime protection**: Container hardening
- **Registry access**: Private ECR

## Compliance

- SOC 2 audit trails
- PCI-DSS secure SDLC
- HIPAA development controls

> See `SECURITY.md` for detailed configurations.
