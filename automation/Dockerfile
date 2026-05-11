FROM python:3.11-slim

# Dépendances système pour SSH et Kubernetes
RUN apt-get update && apt-get install -y --no-install-recommends \
    openssh-client \
    sshpass \
    curl \
    git \
    && curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl" \
    && chmod +x kubectl && mv kubectl /usr/local/bin/ \
    && apt-get clean && rm -rf /var/lib/apt/lists/*

# Installation d'Ansible et des modules K8s/Helm
RUN pip install --no-cache-dir ansible kubernetes

# Répertoire de travail
WORKDIR /gitops
ENV ANSIBLE_HOST_KEY_CHECKING=False

CMD ["sleep", "infinity"]
