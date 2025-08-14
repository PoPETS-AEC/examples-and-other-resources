# examples-and-other-resources

Examples and other resources provided to PETS authors for software artifact
packaging. This repository is itself a demonstration of how to use [git
submodules](#git-submodules).

All the templates or examples written by ourselves are released into the public
domain, so no attribution is needed (see [The Unlicense](LICENSE)). Note that if
you fork some of our examples and build from them to package your own
application, you will likely want to edit the license for [another
one](https://choosealicense.com/).


## Docker and VM Examples


## Resources

### Git Submodules

In order to display the badges and artifacts link next to the paper on the
website, authors need to provide a single URL. However, sometimes the artifacts
are composed or divided into several repositories. A solution consists in using
[git submodules (see
documentation)](https://git-scm.com/book/en/v2/Git-Tools-Submodules) as
demonstrated here on this repository to link to the specific commits of the
other example repositories.

**Note:** users trying to clone a repository with submodules through HTTPs may have
to edit the URL of the submodule if the initial authors specified the SSH URL.
It is possible to avoid this by adding submodules using their relative URL
according to the current repository (see our own [`.gitmodules`](.gitmodules)).

### VS Code and Docker Integration

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

### GNU Parallel

Executing loops in shell to run experiments or trying to execute several jobs in
parallel? Check out the [GNU Parallel](https://www.gnu.org/software/parallel/)
shell tool.


## ToDos
- Python
- Jupyter Notebook
- ML (cuda)
- Golang
- Shadow (VM)
- Renovatebot
- Demonstrate push to DockerHub through GitHub Actions
- git-lfs - zenodo for large file with download script


