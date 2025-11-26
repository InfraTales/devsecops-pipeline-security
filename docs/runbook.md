# Runbook

## Deployment

```bash
npm install && cdk deploy --context environment=prod
```

## Pipeline Stages

1. **Source**: CodeCommit/GitHub trigger
2. **Build**: Compile + unit tests
3. **SAST**: Static analysis (SonarQube/Semgrep)
4. **SCA**: Dependency scan (Snyk/Dependabot)
5. **Container**: Image build + scan
6. **Deploy**: Staging → Production

## Adding Security Gate

```yaml
# buildspec.yml
phases:
  build:
    commands:
      - semgrep --config auto --error
      - snyk test --severity-threshold=high
```

## Monitoring

- Review Security Hub findings daily
- Check pipeline success rates
- Monitor scan duration trends
