# See here for image contents: https://github.com/microsoft/vscode-dev-containers/tree/v0.238.0/containers/alpine/.devcontainer/base.Dockerfile

# [Choice] Alpine version: 3.15, 3.14, 3.13
ARG VARIANT="3.15"
FROM mcr.microsoft.com/vscode/devcontainers/base:0-alpine-${VARIANT} 

RUN apk update \
    && apk add --no-cache python3 py3-pip 
COPY requirements.txt code/
RUN pip install -r code/requirements.txt
