# examples-and-other-resources

Examples and other resources provided to PETS authors for software artifact
packaging.

This repository is itself a demonstration of how to use [git
submodules](resources/git-submodules.md). To clone it, use:

- `git clone --recurse-submodules git@github.com:PoPETS-AEC/examples-and-other-resources.git` (SSH)
- `git clone --recurse-submodules https://github.com/PoPETS-AEC/examples-and-other-resources.git` (HTTPS)


Our resources are nowhere near complete and are only here to facilitate and
demonstrate some ways (others exist!) to package artifacts for authors of
accepted PETS papers. We welcome suggestions in the form of issues or pull
requests.

## License Notes

- These examples are released into the public domain (see [The Unlicense](LICENSE))
- This is to facilitate things, so that authors do not need to give us
  attribution if they re-use our examples.
- Authors who reuse one of our examples as a starter repository, will likely
  want to pick another license for their artifact.

## Docker Examples
- [Python (pip)](https://github.com/PoPETS-AEC/example-docker-python-pip/)
- [Jupyter Notebook (based on Python pip example)](https://github.com/PoPETS-AEC/example-docker-jupyter-notebook/)
- [Golang](https://github.com/PoPETS-AEC/example-docker-golang/)

## Other Resources
- [Building the Docker image with a GitHub Action workflow](resources/github-workflow-docker-image.md)
- [Git Submodules](resources/git-submodules.md)
- [GNU Parallel](resources/gnu-parallel.md)
- [Large files solutions](resources/large-files-solutions.md)
- [Licenses](resources/licenses.md)
- [Dependabot and Renovate](resources/dependabot-renovate-bot.md)
- [VS Code and Docker Integration](resources/vs-code-docker-integration.md)


## ToDos

Docker:
- [ ] C
- [x] Golang
- [x] Jupyter Notebook
- [ ] Python (conda)
- [x] Python (pip)
- [ ] Python (uv)
- [ ] Python ML workflow with cuda and GPU acceleration
- [ ] Rust
- [ ] Docker Compose Example

Other:
- [ ] Shadow (Tor) - VM?
- [ ] NixOS examples
- [ ] Automate Zenodo dataset download with script in an example repo

