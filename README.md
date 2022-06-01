# pocket-missile

## Building

```bash
# Building the kernel
cargo build

# Linking the kernel to a virtual bootloader
cargo install bootimage
cargo bootimage

# Run tests against a VM with qemu
cargo test
```

## Virtualize `pocket-missile` with qemu

`cargo` is configured to run `qemu` in headless mode (see
`package.metadata.bootimage` in [Cargo.toml][]). If you have VSCode
(and/or Docker), run the container in [.devcontainer][] and `cargo` will
virtualize the kernel with `qemu` __inside__ the container.

[Cargo.toml]: ./Cargo.toml
[.devcontainer]: ./devcontainer