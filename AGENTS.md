# AGENTS.md

Base image for the CruGlobal-AI AppBuilder services: `ghcr.io/cruglobal-ai/service-cli:{master,develop}`.

- Upstream `digiserve/service-cli` exists only on Docker Hub. There is no public source repo.
- For now `.github/workflows/mirror.yml` copies the upstream tags into GHCR (weekly, on push, or by hand).
- Services build with `FROM ghcr.io/cruglobal-ai/service-cli:${BRANCH}`.
- Plan: swap the mirror for a real `Dockerfile` here once we own the base image.
