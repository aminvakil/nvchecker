# nvchecker
New version checker for software releases

This repository includes upstream packages and docker images which I use to maintain my AUR packages and docker images.

It runs daily to check for updates and creates pull requests when updates are available.

## Scope

This repository is maintained for my personal package and image tracking. It is not intended as a shared package registry, and pull requests adding packages for other people are not accepted. If you want to track your own packages, please fork the repository and customize the `*.toml` files and workflows for your own use.

## Automated bump branches

The workflows create pull requests using these branch naming conventions:

- AUR package bumps: `aurbump-<name>`
- Other package bumps: `othersbump-<name>`
- Docker image bumps in this repository: `dockerbump-<name>`
- Docker image bumps in external repositories: existing per-image branches such as `alpine`, `golang`, and `archlinux`
