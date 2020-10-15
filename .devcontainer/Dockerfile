# See here for image contents: https://github.com/microsoft/vscode-dev-containers/tree/v0.145.0/containers/python-3/.devcontainer/base.Dockerfile

# [Choice] Python version: 3, 3.8, 3.7, 3.6
ARG VARIANT="3"
FROM mcr.microsoft.com/vscode/devcontainers/python:0-${VARIANT}

RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install --no-install-recommends pdns-server pdns-backend-pipe dnsutils \
    && pip3 --disable-pip-version-check --no-cache-dir install --quiet mock assertpy pytest
