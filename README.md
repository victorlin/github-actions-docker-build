# github-actions-docker-build

Automatically build a Docker image on GitHub Actions, hosted on GitHub Container Registry

## 1. Setup

Fork this repository, or add all its contents into an existing repository. You
will need a GitHub account to continue.


## 2. Customize the image

The [Dockerfile] defines the Docker image.. Refer to [Docker Docs] for examples
on how to make changes to this file.

Once the Dockerfile has been updated on GitHub, it will automatically trigger a
build of the image on GitHub Container Registry as an image tagged with the
repository's name and owner.

> [!NOTE]
> The first push in a repository may fail due to lack of GitHub permissions on a
> package that hasn't been created yet. Subsequent pushes should succeed.

[Dockerfile]: ./Dockerfile
[Docker Docs]: https://docs.docker.com/build/building/packaging/
