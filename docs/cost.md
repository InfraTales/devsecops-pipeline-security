# Cost Analysis (₹)

Cost estimates for **DevSecOps Pipeline Security** in **Indian Rupees (₹)**.

## Production Environment

| Service | Monthly Cost (₹) | Notes |
|---------|------------------|-------|
| **CodePipeline** | ₹8,000–15,000 | Pipeline executions |
| **CodeBuild** | ₹10,000–25,000 | Build minutes |
| **ECR** | ₹3,000–8,000 | Container images |
| **Security Hub** | ₹5,000–12,000 | Findings aggregation |
| **Inspector** | ₹8,000–20,000 | Vulnerability scanning |
| **Secrets Manager** | ₹2,000–5,000 | Secret storage |
| **Total** | **₹36,000–85,000** | ~$450–1,060/month |

## Per-Pipeline Costs

| Pipeline Type | Cost per Run (₹) |
|--------------|------------------|
| Simple (lint + test) | ₹10–20 |
| Full SAST/DAST | ₹50–100 |
| Container scan | ₹30–60 |

## Cost Optimization

- **Cache dependencies** – Reduce build time
- **Parallel stages** – Faster feedback
- **Scheduled scans** – Off-peak hours
- **Incremental analysis** – Scan only changes
