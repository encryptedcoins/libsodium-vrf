# libsodium-vrf

The library wanted for compiling `encoins-relay` packages on Arch-like OS.

`encoins-relay` depends on `cardano-base` which depend on `cardano-crypto-praos` which depends on [dynamically linking](https://github.com/input-output-hk/cardano-base#without-nix) `libsodium` and `libsodium-vrf`.

The last one is just [available](https://github.com/input-output-hk/iohk-nix/releases/tag/v2.2) as `deb`. Therefore we made `encoins-relay` to pick up `libsodium-vrf` via Setup.hs from submodules.
