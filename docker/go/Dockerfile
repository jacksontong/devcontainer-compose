FROM mcr.microsoft.com/vscode/devcontainers/go:1.23-bookworm

USER vscode

RUN go install github.com/air-verse/air@latest && \
    go install golang.org/x/tools/cmd/godoc@latest && \
    go install golang.org/x/pkgsite/cmd/pkgsite@latest

RUN sh -c "$(wget -O- https://github.com/deluan/zsh-in-docker/releases/download/v1.2.0/zsh-in-docker.sh)" -- \
    -p git \
    -p https://github.com/zsh-users/zsh-autosuggestions