# Git Submodules

In order to display the badges and artifacts link next to the paper on the
website, authors need to provide a single URL. However, sometimes the artifacts
are composed or divided into several repositories. A solution consists in using
[git submodules (see
documentation)](https://git-scm.com/book/en/v2/Git-Tools-Submodules) as
demonstrated here on this repository to link to the specific commits of the
other example repositories.

**Note:** users trying to clone a repository with submodules through HTTPs may
have to edit the URL of the submodule if the initial authors specified the SSH
URL. It is possible to avoid this by adding submodules using their relative URL
according to the current repository (see our own [`.gitmodules`](../.gitmodules)).
