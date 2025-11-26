# Troubleshooting

## Common Issues

### Pipeline Fails at Security Gate
- Review scan findings
- Check severity thresholds
- Add exceptions if false positive

### Slow Scans
- Enable caching
- Use incremental scanning
- Parallelize stages

### False Positives
- Configure ignore rules
- Update scanner rules
- Add inline suppressions

### Secrets Detected
- Rotate exposed secrets immediately
- Add to .gitignore
- Use Secrets Manager
