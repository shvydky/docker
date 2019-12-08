# Docker Builders
This repository contains sources of build images.
All images are based on [docker](https://hub.docker.com/_/docker) image to allow docker-in-docker execution.

| Platform | Docker Image | Dockerfile |
| -------- | ------------ | ---------- |
| .NET Core 3.1 | `shvydky/builders:dotnet-3.1` | [/dotnet/3.1/Dockerfile](/dotnet/3.1/Dockerfile) |
| .NET Core 2.2 | `shvydky/builders:dotnet-2.2` | [/dotnet/2.2/Dockerfile](/dotnet/2.2/Dockerfile) |
| NodeJS 12.13.0 | `shvydky/builders:node-12.13` | [/node/12.13/Dockerfile](/node/12.13/Dockerfile) |