# A16_RISCV/external/crosvm: android16-riscv

Changes made for the Android 16 (AOSP, riscv64) bring-up of the BananaPi BPI-F3 (SpacemiT K1) and the BananaPi BPI-SM10 (SpacemiT K3), on branch `android16-riscv`.

crosvm for riscv64 (AVF on the K3, which has the H extension).

## Changes

- **Enable crosvm for riscv64**: Allow the crosvm rust defaults on riscv64 so the virt APEX can ship crosvm on RISC-V SoCs with the H extension (SpacemiT K3).

## Build

```
./build.sh k1   # BPI-F3 (K1): kernel, bootloaders and Android images
./build.sh k3   # BPI-SM10 (K3), not booted yet
```

`./build.sh --help` lists the options (`--skip-kernel`, `--kernel-only`, ...).
