# Test repo for issue numtide/treefmt-nix#78

## Init

    nix flake init -t github:hercules-ci/flake-parts

## Add treefmt

Add
    treefmt-nix.url = "github:numtide/treefmt-nix";

inside mkFlake

    imports = [
      inputs.treefmt-nix.flakeModule
    ];

## Run command twice

nix flake show
