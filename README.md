    # bfstore Platform GitOps

    GitOps deployment configuration for bfstore services, including Kubernetes manifests, environment overlays, release workflows, and operational deployment patterns.

    ## Repository status

    This repository is an early bfstore portfolio repository. It is currently being set up with initial structure, documentation, and direction before implementation work begins.

    ## Purpose

    This repository will hold the desired deployment state for bfstore services and platform components running on Kubernetes.

    bfstore is a cloud-native ecommerce platform for developer-themed homeware. This repository is part of the wider bfstore portfolio and is intended to demonstrate senior platform engineering, DevSecOps, Kubernetes, cloud infrastructure, and developer experience capability.

    ## Scope

    This repository will cover:

    - Kubernetes application definitions
- Environment overlays
- GitOps deployment workflows
- Release promotion patterns
- Ingress, gateway, and service routing configuration
- Operational manifests for observability and platform services

    ## Out of scope

    This repository will not own:

    - Application source code
- Cloud infrastructure provisioning
- Reusable Terraform modules
- Security policy source-of-truth where policies belong in governance repos

    ## Suggested repository structure

    - `apps/                 # bfstore application deployment definitions`
- `platform/             # Shared platform component manifests`
- `envs/                 # Environment overlays`
- `docs/                 # GitOps operating model and ADRs`
- `scripts/              # Local validation helpers`

    ## Initial roadmap

    - [ ] Select initial GitOps tool direction
- [ ] Define local, dev, staging, and production environment layout
- [ ] Add first service deployment pattern
- [ ] Add health, rollout, and rollback guidance
- [ ] Document promotion workflow

    ## Engineering principles

    - Prefer simple, repeatable workflows over clever one-off scripts.
    - Document trade-offs clearly.
    - Keep security and operability visible from the beginning.
    - Design for local development first, then cloud deployment.
    - Treat naming, conventions, and structure as production foundations.

    ## Related bfstore repositories

    ```text
    bfstore
      Main ecommerce microservices platform.

    bfstore-platform-infra
      Cloud infrastructure foundations.

    bfstore-platform-gitops
      Kubernetes GitOps deployment state.

    bfstore-terraform-modules
      Reusable Terraform modules.

    bfstore-security-governance
      Security, compliance, policy, and governance controls.

    bfstore-developer-platform
      Golden paths, templates, and developer experience tooling.
    ```

    ## GitHub topics

    ```text
    gitops kubernetes argocd flux helm kustomize platform-engineering devops continuous-delivery sre bfstore
    ```

    ## Practical rule

    Keep it boring where production matters.
