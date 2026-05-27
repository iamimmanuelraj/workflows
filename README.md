# Workflows

Public repo for running GitHub Actions on private projects (free minutes).

Each workflow clones a private repo (stored as a secret), runs its job, and pushes results back.

## Adding a new project

1. Add a workflow file: `.github/workflows/<project>.yml`
2. Add secrets: `<PREFIX>_REPO` (e.g. `iamimmanuelraj/my-private-repo`) + any project-specific secrets
3. All workflows share `GH_TOKEN` (PAT with repo access)
