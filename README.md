# GitHub Actions runner (Ubuntu 24.04)

An ephemeral GitHub action runner in a Docker container. 

This container is automatically checked weekly and updated with the latest
version of [actions runner](https://github.com/actions/runner).

See [packages](https://github.com/Onvox/actions-runner-ubuntu2404/pkgs/container/actions-runner-ubuntu2404) 
for the available runner version tags.

## Getting Started

```
$ docker pull ghcr.io/onvox/actions-runner-ubuntu2404:<version_tag>
```

See [docker-compose.yml.example](docker-compose.yml.example) for an
example docker compose configuration.

## Configuration

A minimum configuration consists of setting the following environment variables:

* `GITHUB_ORG`: "MyGitHubOrganization"  # GitHub Organization name
* `GITHUB_TOKEN`: ghp_superSecretKey    # GitHub token with admin:org
