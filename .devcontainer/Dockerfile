# Use Ubuntu as base
FROM mcr.microsoft.com/vscode/devcontainers/base:ubuntu-22.04

# Install Ansible + Docker client
RUN apt-get update && \
    apt-get install -y --no-install-recommends \
        software-properties-common \
        python3 python3-pip python3-venv \
        ansible \
        docker.io \
        sshpass \
        git && \
    apt-get clean && rm -rf /var/lib/apt/lists/*

# Default shell
CMD ["/bin/bash"]
