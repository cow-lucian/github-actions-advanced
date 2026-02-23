# GitHub Actions Advanced

Advanced GitHub Actions patterns - container jobs, service containers, dynamic matrices, self-hosted runners, composite actions, reusable workflows, OIDC, security hardening, triggers, secrets management, GitHub App & OAuth App authentication, and custom webhook events.

## Workflow Catalog

| # | File | Topic | Level |
|---|------|-------|-------|
| 01 | `01-container-jobs.yml` | Docker container jobs, volumes, ports, private registries | Advanced |
| 02 | `02-services.yml` | Service containers - PostgreSQL, Redis, LocalStack, MailHog | Advanced |
| 03 | `03-dynamic-matrix.yml` | Dynamic matrix generation from files, APIs, git diffs | Advanced |
| 04 | `04-self-hosted-runners.yml` | Self-hosted runners, labels, groups, ephemeral, security | Advanced |
| 05 | `05-composite-run-steps.yml` | Composite actions with inputs, outputs, conditional logic | Advanced |
| 06 | `06-reusable-workflow-caller.yml` | Calling reusable workflows with inputs, outputs, secrets | Advanced |
| 07 | `07-oidc-cloud-auth.yml` | OIDC keyless auth for AWS, Azure, GCP | Advanced |
| 08 | `08-security-hardening.yml` | Pinned actions, permissions, Scorecard, supply chain | Advanced |
| 09 | `09-all-triggers-reference.yml` | **Multi-trigger workflows, event routing, concurrency** | Advanced |
| 10 | `10-secrets-auth-deepdive.yml` | **Auth hierarchy, OIDC internals, GitHub App JWT flow** | Advanced |
| 11 | `11-github-app-oauth-setup.yml` | **GitHub App & OAuth App complete setup and comparison** | Advanced |
| 12 | `12-custom-webhooks-events.yml` | **External webhooks, Stripe/PagerDuty/Slack integration** | Advanced |

## New Content Highlights

### Triggers & Event Patterns (09)
- Multi-trigger workflows combining push, PR, schedule, release, dispatch
- Event router pattern - different jobs based on trigger type
- Advanced concurrency control per trigger type
- Trigger context differences (SHA, ref, filters per event)

### Secrets & Authentication Deep Dive (10)
- Complete authentication hierarchy (GITHUB_TOKEN -> App -> PAT -> OIDC)
- GITHUB_TOKEN internals and permission testing
- GitHub App JWT generation flow with diagrams
- OIDC token claims and cloud provider setup (AWS, Azure, GCP)
- Token audit checklist and rotation patterns

### GitHub App & OAuth App Setup (11)
- Step-by-step GitHub App creation guide
- Permission reference (all repository and organization permissions)
- Private key generation and secret storage
- 5 practical usage patterns (cross-repo, protected branches, workflow triggers)
- Complete OAuth 2.0 flow diagram (web and device flow)
- OAuth scopes reference (all 30+ scopes)
- Decision tree for choosing authentication method
- Security comparison matrix

### Custom Webhooks & Events (12)
- External webhook integration (Stripe, PagerDuty, Slack)
- Middleware server patterns (Node.js, Python)
- Idempotency patterns for duplicate webhook handling
- Event routing and validation
- ChatOps via repository_dispatch

## Related Repositories

| Repository | Description |
|------------|-------------|
| [github-actions-examples](https://github.com/cow-lucian/github-actions-examples) | Beginner to intermediate: triggers, expressions, job/step features |
| [custom-actions](https://github.com/cow-lucian/custom-actions) | Custom action development: composite, JavaScript, Docker |
| [reusable-workflows](https://github.com/cow-lucian/reusable-workflows) | Reusable workflow library: CI, deploy, Docker, security, notifications |

## License

MIT
