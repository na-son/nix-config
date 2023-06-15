# Nix Flake configuration

Currently untested with macos.

Intended to be the contents of `/etc/nixos` currently.

A new platform in `./platforms` needs to be created for new hardware hosts.

Heavily inspired by [hoverbear](https://github.com/Hoverbear-Consulting/flake)

## Checks / tests

Deadnix, checks unused code / lambdas

```shell-session
nix run github:astro/deadnix .
```

Statix, style / antipattern checker

```shell-session
nix run nixpkgs#statix check .
```

