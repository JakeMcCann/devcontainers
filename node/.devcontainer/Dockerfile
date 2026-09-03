FROM mcr.microsoft.com/devcontainers/typescript-node:22-bookworm

RUN apt-get update \
    && apt-get install --yes --no-install-recommends ripgrep \
    && rm -rf /var/lib/apt/lists/*

RUN su node -c "umask 0002 && npm install --global opencode-ai" \
    && su node -c "opencode --version"
