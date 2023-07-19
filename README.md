# Test linting with flake-parts

## Init

    nix flake init -t github:hercules-ci/flake-parts

## Add treefmt

Add
    treefmt-nix.url = "github:numtide/treefmt-nix";

inside mkFlake

    imports = [
      inputs.treefmt-nix.flakeModule
    ];
