# MLOps Platform

Catalog-based, multi-tenant MLOps platform using GitOps principles.

## Structure
- catalog/  → platform-managed components
- tenants/  → team-specific overlays

## Usage
Each tenant directory can be deployed via Kustomize or ArgoCD.

Example:
```bash
kubectl apply -k tenants/team-alpha
