# Copilot Instructions for acme-04-platform Infrastructure (AWS)

This is the AWS infrastructure repository for acme-04-platform.

## Tech Stack

- Terraform
- AWS
- tflint for linting

## Available Agents

| Agent | Purpose |
|-------|--------|
| `@infra` | Infrastructure design, Terraform, deployment |
| `@security` | Security review and hardening |
| `@infra-orchestrator` | Issue and sprint management |

## Commands

```bash
terraform init       # Initialize
terraform plan       # Preview changes
terraform apply      # Apply changes
terraform validate   # Validate config
tflint              # Lint
```

## Project Structure

```
terraform/
├── environments/    # Per-environment configs
│   ├── dev/
│   ├── staging/
│   └── prod/
├── modules/        # Reusable modules
└── shared/         # Shared resources
```
