# Deno Actions

This repository holds a couple of useful GitHub Actions for working with Deno.
The actions are:

- CI (ci.yml): Run tests, format and linting checks on your Deno project
- Build Docker Container (build-docker-container.yml): Build a Docker container
  for your Deno project.
- Build OCI Container (build-oci-container.yml): Build a OCI compliant container
  for your Deno project. It is built with Buildah which creates a container
  image that is also possible to run with Docker or Podman.
- Build Multi Arch Docker Container (build-multi-arch-docker-container.yml):
  Build a Docker container for your Deno project. It is built with Buildx which
  creates a multi-arch container image that can run on different architectures.
  In this case it will output an `arm64` and `amd64` container image.
- Coverage (coverage.yml): Generate a coverage report for your Deno project and
  uploads it onto Github Pages to
  [`https://<YourUsername>.github.io/<RepositoryName>/index.html`](https://<YourUsername>.github.io/<RepositoryName>/index.html).
- Deploy to Deno Deploy (deno-deploy.yml): Deploy your Deno project to Deno
  Deploy.

You can find the workflows in the `.github/workflows` directory.
