FROM mcr.microsoft.com/devcontainers/typescript-node:22-bookworm

RUN su node -c "umask 0002 && npm install --global opencode-ai" \
    && su node -c "opencode --version"
