# GitHub Workflow and Container Registry (and/or DockerHub)

Some of our example repositories (like [this
one](https://github.com/PoPETS-AEC/example-docker-python-pip)) directly
demonstrate how to use a GitHub Action workflow to build and push a Docker image
to a registry.

For the linked repository above, a workflow triggers every time a new commit
modifies the `Dockerfile` (this can easily be switched to trigger on other
conditions). This workflow is configured to automatically build and push the
Docker image to GitHub's Container Registry.

As a result, there is no need to manually build the image locally, as it can
instead be pulled and used from the Container Registry (verify that the
package's visibility is set to `Public`):

```bash
docker pull ghcr.io/edit-namespace/edit-image-name:edit-tag

docker run --rm -it -v ${PWD}:/workspaces/example \
    -w /workspaces/example \
    --entrypoint bash ghcr.io/edit-namespace/edit-image-name:edit-tag
```

Similarly, it is also possible to push the image to the DockerHub, we defer to
the documentation provided by GitHub
[here](https://docs.github.com/en/actions/tutorials/publish-packages/publish-docker-images)
for more details. Note that for DockerHub, an account username and access tokens
are required and should be provided as a repository variable and a secret,
respectively, for the workflow to be able to use them.