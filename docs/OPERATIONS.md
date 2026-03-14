# Operations

## Deployment flow (GitOps)

1. App image built and pushed by app repo CI.
2. GitOps CD updates image tag in gitops/apps/*/overlays.
3. Argo CD/Flux syncs clusters/clusters/* to clusters.
4. Changes are audited via git history.

## Incident response (example)

- Check dashboards in Grafana.
- Inspect alerts in Alertmanager.
- Investigate logs via Loki/ELK.
- Use kubectl describe/logs for pod-level details.
