# Kubernetes Standards

- All workloads must define requests/limits.
- Readiness and liveness probes are mandatory for HTTP workloads.
- ServiceAccounts and Roles are required; avoid default SA.
- NetworkPolicy default-deny + explicit allows per app.
- All secrets managed via external secret manager or SealedSecrets.
- CI must validate manifests (kubeconform + kustomize build).
