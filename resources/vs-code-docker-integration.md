# VS Code and Docker Integration

Some of our example repositories (like [this
one](https://github.com/PoPETS-AEC/example-docker-python-pip)) directly
demonstrate this integration. Here is what you need to make it work:

**Requirements:**
- [VS code](https://code.visualstudio.com/download)
- [VS code Dev Containers
  extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)
- [Docker Engine](https://docs.docker.com/engine/install/)

**Setup:**
1. Open the command palette in VS Code (CTRL+SHIFT+P).
2. Select `Dev-Containers: Open Folder in Container...` and choose the
   project directory.
3. VS Code deploys the container and mounts the project directory as a volume
   automatically. Just open a terminal in VS Code (CTRL+SHIFT+`) to run
   commands.

**Miscellaneous:**
- To rebuild the image, open the command palette (CTRL+SHIFT+P), and select
  `Dev-Containers: Rebuild and reopen in container`
- You can customize VS Code settings through the `devcontainer.json` file under
  `.devcontainer/`
- There is a useful [Dev Container
  CLI](https://code.visualstudio.com/docs/devcontainers/devcontainer-cli) that
  lets you (among other things) open VS Code directly with the corresponding
  container launched.