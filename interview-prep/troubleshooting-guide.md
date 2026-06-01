# Troubleshooting Guide — Concise

Summary

A compact checklist and examples to diagnose common cloud incidents quickly.

Checklist

1. Reproduce and scope: who/what/when is affected?
2. Check logs: app logs, CloudWatch, journalctl, pod logs.
3. Resource utilization: CPU, memory, disk (`df -h`, `kubectl top`).
4. Network & DNS: ping, traceroute, dig.
5. Recent changes: deployments, config, infra updates.

Scenarios

- Web app 500 errors: check app logs, health checks, and recent deployments.
- High latency: check CPU/memory, DB slow queries, and network metrics.
- Failed deployment: inspect CI logs and rollback if needed.

Related topics

- AWS core: ../aws/aws-core-services.md
- Kubernetes debugging: ../kubernetes/kubernetes-basics.md
