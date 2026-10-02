# cf-amazon-connect

A hands-on exercise: rebuilding pieces of the `cdk-amazon-connect` demo project directly in raw AWS CloudFormation (YAML), instead of through CDK — to see the same resources, written the other way.

Companion/reference project: [cdk-amazon-connect](https://github.com/PratikTamboli/cdk-amazon-connect).

## Deploying

```bash
aws cloudformation deploy \
  --template-file templates/<name>.yaml \
  --stack-name <stack-name> \
  --capabilities CAPABILITY_NAMED_IAM
```

## Structure

- `templates/` — CloudFormation YAML templates, built up one resource at a time.
