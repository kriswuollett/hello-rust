# Rust Getting Started

The code and any follow up explorations from following the [Rust Getting Started Guide](https://www.rust-lang.org/learn/get-started).

## Installation

```console
kris@slate ~ % curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh

info: downloading installer

Welcome to Rust!

This will download and install the official compiler for the Rust
programming language, and its package manager, Cargo.

Rustup metadata and toolchains will be installed into the Rustup
home directory, located at:

  /Users/kris/.rustup

This can be modified with the RUSTUP_HOME environment variable.

The Cargo home directory located at:

  /Users/kris/.cargo

This can be modified with the CARGO_HOME environment variable.

The cargo, rustc, rustup and other commands will be added to
Cargo's bin directory, located at:

  /Users/kris/.cargo/bin

This path will then be added to your PATH environment variable by
modifying the profile files located at:

  /Users/kris/.profile
  /Users/kris/.bash_profile
  /Users/kris/.zshenv

You can uninstall at any time with rustup self uninstall and
these changes will be reverted.

Current installation options:


   default host triple: x86_64-apple-darwin
     default toolchain: stable (default)
               profile: default
  modify PATH variable: yes

1) Proceed with installation (default)
2) Customize installation
3) Cancel installation
>1

info: profile set to 'default'
info: default host triple is x86_64-apple-darwin
info: syncing channel updates for 'stable-x86_64-apple-darwin'
info: latest update on 2021-05-10, rust version 1.52.1 (9bc8c42bb 2021-05-09)
info: downloading component 'cargo'
info: downloading component 'clippy'
info: downloading component 'rust-docs'
info: downloading component 'rust-std'
 23.0 MiB /  23.0 MiB (100 %)  21.5 MiB/s in  1s ETA:  0s
info: downloading component 'rustc'
 58.6 MiB /  58.6 MiB (100 %)  21.7 MiB/s in  2s ETA:  0s
info: downloading component 'rustfmt'
info: installing component 'cargo'
info: using up to 500.0 MiB of RAM to unpack components
info: installing component 'clippy'
info: installing component 'rust-docs'
 15.3 MiB /  15.3 MiB (100 %)   6.3 MiB/s in  1s ETA:  0s
info: installing component 'rust-std'
 23.0 MiB /  23.0 MiB (100 %)   8.4 MiB/s in  4s ETA:  0s
info: installing component 'rustc'
 58.6 MiB /  58.6 MiB (100 %)   3.6 MiB/s in 14s ETA:  0s
info: installing component 'rustfmt'
info: default toolchain set to 'stable-x86_64-apple-darwin'

  stable-x86_64-apple-darwin installed - rustc 1.52.1 (9bc8c42bb 2021-05-09)


Rust is installed now. Great!

To get started you may need to restart your current shell.
This would reload your PATH environment variable to include
Cargo's bin directory ($HOME/.cargo/bin).

To configure your current shell, run:
source $HOME/.cargo/env
```

## Generating a new project

```console
kris@slate kriswuollett % cargo new hello-rust
     Created binary (application) `hello-rust` package
kris@slate kriswuollett % cd hello-rust 
kris@slate hello-rust % cargo run
   Compiling hello-rust v0.1.0 (/Users/kris/workspace/kriswuollett/hello-rust)
    Finished dev [unoptimized + debuginfo] target(s) in 1.35s
     Running `target/debug/hello-rust`
Hello, world!
```

