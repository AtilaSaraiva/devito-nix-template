# Devito Nix python template

This is my personal template for a devito development environment, using [Nix](https://nixos.org/). I use [niv](https://github.com/nmattia/niv) for pinning the nixpkgs repository revision, hence pinning the dependencies of the project.

## Making the development environment available

Using [nix](nixos.org), run:

```shell
  git clone https://github.com/<youruser>/<repo-name>.git
  cd <repo-name>
  nix-shell
```

and a shell with all the necessary dependencies will appear.

## To update the dependencies

This template uses [niv](https://github.com/nmattia/niv) to pin the revision of the nixpkgs repository, but eventually it will be necessary to work with the newer versions of the project dependencies. To do that simply run:

```shell
  niv update
```
