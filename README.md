# pocket-missile

## Building

```bash
# Building the kernel
cargo build

# Linking the kernel to bootloader
cargo install bootimage
cargo bootimage
```

## Run with QEMU

```bash
qemu-system-x86_64 -drive format=raw,file=target/x86_64-pocket-missile/debug/bootimage-pocket-missile.bin
```