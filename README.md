# extract-docker-tag

## Usage

You can use this action inside your ci workflow by adding the following steps to the job responsible for building docker image

```
- name: Push Docker image with tag "${{ env.DOCKER_TAG }}"
  run: make docker-push
```