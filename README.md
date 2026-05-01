# IT Infrastructure/GitOps focus - Flux CD


## Description
`Test project designed for GitOps operations and continuous delivery of infrastructures and microservices applications. This repository centralizes CI/CD workflows, Infrastructure as Code (IaC) configurations, and Kubernetes deployment management.

## Architecture & Stack
- **Orchestration :** Kubernetes (Kind/Production)
- **GitOps :** Flux CD (Pull model)
- **IaC :** Terraform / Ansible
- **CI/CD :** GitHub Actions


## Structure du Projet
```text
.
├── .github/workflows/   # CI Pipelines
├── clusters/            # Définitions Kubernetes (Kustomize/Helm)
├── infrastructure/      # Scripts Terraform / Ansible
├── scripts/             # Utilitaires de déploiement
└── README.md
