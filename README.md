# DevOps/IT Infrastructure/GitOps focus


## Description
`rt-ops-delivery` est un framework d'automatisation des opérations (GitOps) conçu pour le déploiement continu d'infrastructures et d'applications microservices. Ce dépôt centralise les workflows CI/CD, les configurations IaC (Infrastructure as Code) et la gestion des déploiements Kubernetes.

## Architecture & Stack
- **Orchestration :** Kubernetes (Kind/Production)
- **GitOps :** Flux CD (Pull model)
- **IaC :** Terraform / Ansible
- **CI/CD :** GitHub Actions
- **Infrastructure :** Linux Hardened Repositories, Veeam integration, Networking (Sophos/Azure)

## Structure du Projet
```text
.
├── .github/workflows/   # CI Pipelines
├── clusters/            # Définitions Kubernetes (Kustomize/Helm)
├── infrastructure/      # Scripts Terraform / Ansible
├── scripts/             # Utilitaires de déploiement
└── README.md
