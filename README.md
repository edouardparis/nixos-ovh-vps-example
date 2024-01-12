# nixos-ovh-vps-example

Minimal flake to use for a 2GB ovh vps
Change configuration in `disk-config.nix` and `configuration.nix` 

test:

```
nix run github:nix-community/nixos-anywhere -- --flake .#ovh-vps --vm-test
```

deploy:
```
nix run github:nix-community/nixos-anywhere -- --flake .#ovh-vps root@<vps-ip>
```
