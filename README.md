# Installation
1. Clone this repository
2. Register the hooks using `git config --global core.hooksPath /path/to/this/repository/githooks`

# Hooks
## post-checkout
This will automatically pull from remote after checking out a branch.
Additionally it will try to update your local vendor-dependencies for go and php projects.

## pre-push
This will automatically run checks for go projects (test, vet, gofumpt, misspell, unconvert, staticcheck, ineffassign, unparam)

## pre-commit
This will automatically check for go projects if the dependencies are up-to-date
