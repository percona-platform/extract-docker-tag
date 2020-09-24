# extract-docker-tag

This action runs a go script to extract the docker image tag and set it as the value of `DOCKER_TAG` environment variable that can be used by other workflows.

## Usage

You can use this action inside your ci workflow by adding the following steps to the job responsible for building docker image

```
- name: Push Docker image with tag "${{ env.DOCKER_TAG }}"
  run: make docker-push
```