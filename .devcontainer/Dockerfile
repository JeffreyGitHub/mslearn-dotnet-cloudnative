
# Base image: Uses the official Dev Containers base for Ubuntu 22.04 (“Jammy”).
# Jammy is Ubuntu version name where 22.04 is version number  
FROM mcr.microsoft.com/devcontainers/base:jammy 
  
# Install .NET 8 SDK
RUN wget https://packages.microsoft.com/config/ubuntu/22.04/packages-microsoft-prod.deb -O packages-microsoft-prod.deb \
    && dpkg -i packages-microsoft-prod.deb \
    && rm packages-microsoft-prod.deb \
    && apt-get update \
    && apt-get install -y dotnet-sdk-8.0

# Install Docker CE (includes docker, buildx, compose)
# Docker CE (Community Edition) is the free, open‑source version of Docker,
# It provides all the core containerization capabilities needed to build, run, and manage containers on your local machine. 
# The same engine that powers containers across Linux (called Docker CE), macOS, and Windows (called Docker Engine)

# RUN apt-get update \
#     && apt-get install -y ca-certificates curl gnupg lsb-release \
#     && install -m 0755 -d /etc/apt/keyrings \
#     && curl -fsSL https://download.docker.com/linux/ubuntu/gpg | gpg --dearmor -o /etc/apt/keyrings/docker.gpg \
#     && chmod a+r /etc/apt/keyrings/docker.gpg \
#     && echo \
#        "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.gpg] \
#        https://download.docker.com/linux/ubuntu \
#        $(lsb_release -cs) stable" | tee /etc/apt/sources.list.d/docker.list > /dev/null \
#     && apt-get update \
#     && apt-get install -y docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin

# docker-ce: Docker daemon, Pulling images, running containers, manage networks and volumes
# docker-ce-cli
# containerd.io:  Container runtime and API

# docker-buildx-plugin: is a Docker CLI plugin that provides advanced image‑building features using BuildKit.
# docker-compose-plugin:  is a tool for defining and running multi‑container applications using a YAML file.