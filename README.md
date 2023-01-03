## Flake-based development shell for Nix


### Instructions

- Make sure you have installed Nix and have [enabled Nix flakes](https://nixos.wiki/wiki/Flakes) in your local environment.

- Fork project as template.

- Then `git clone` on your project fork

- After putting your dependencies in `shell.nix`, run `flake develop` to initialize project (if you have `direnv`, then run `direnv allow` and thereafter the project will be initialized automatically when you `cd` into that directory)

### Nix package source

I have this flake pinned to my fork of `nixpkgs`, but you are free to change the `nixpkgs` to the original `NixOS` `nixpkgs`, or any other fork or commit that you wish. The settingi to change is `inputs.nixpkgs.url` (same applies to my fork of `flake-utils`, which is this project's only dependency outside of Nix itself).

### Dependencies

The template only has `jq` as a project dependency, but you are free to use any project dependency that is available in recent `nixpkgs`.

### License

Dual-licensed under MIT or the UNLICENSE.
