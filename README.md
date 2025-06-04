# Andromeda 🌌

<a href="https://github.com/load1n9/andromeda"><img align="right" src="./assets/andromeda.svg" alt="Andromeda" width="150"/></a>

[![Discord Server](https://img.shields.io/discord/1264947585882259599.svg?logo=discord&style=flat-square)](https://discord.gg/tgjAnX2Ny3)

The simplest JavaScript and TypeScript runtime, fully written in
[Rust 🦀](https://www.rust-lang.org/) and powered [Nova](https://trynova.dev/).

> Note: ⚠️ This project is still in early stages and is not suitable for serious
> use.

## Installation

The easiest way to install Andromeda is to have
[Cargo](https://doc.rust-lang.org/cargo/) installed and run the following
command:

```bash
cargo install --git https://github.com/tryandromeda/andromeda
```

## Getting Started

To get started with Andromeda, follow these steps:

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/tryandromeda/andromeda
   cd andromeda
   ```

2. **Install**

   ```bash
   cargo install --path ./cli
   ```

---

## Usage

To run a JavaScript or TypeScript file, use the following command:

```bash
andromeda run <file>
```

### Interactive REPL

Andromeda includes an interactive REPL (Read-Eval-Print Loop) for testing JavaScript or TypeScript code quickly:

```bash
# Start the REPL
andromeda repl

# REPL with debugging options
andromeda repl --print-internals --expose-internals
```

**REPL Commands:**

- Type JavaScript code and press Enter to evaluate
- Type `exit` to quit
- Type `gc` to trigger garbage collection
- Press Ctrl+C to exit

**REPL Options:**

- `--expose-internals`: Expose Nova internal APIs for debugging
- `--print-internals`: Print internal debugging information  
- `--disable-gc`: Disable garbage collection

## Crates

| Crate                         | Description                                               |
| ----------------------------- | --------------------------------------------------------- |
| [andromeda](/cli)             | Contains the Executable Command Line Interface (CLI) code |
| [andromeda-core](/core)       | Contains the core runtime code                            |
| [andromeda-runtime](/runtime) | Contains the runtime code                                 |

[Mozilla Public License Version 2.0](./LICENSE.md)
