# dbgeng-sys

Low-level Rust FFI bindings to the Windows Debugger Engine (`dbgeng.dll`).

## Overview

This crate links to `dbgeng` and `dbghelp`, allowing direct access to WinDBG APIs from Rust.

## Requirements

- Windows OS
- Windows 10 SDK (Debugging Tools)
- Rust (edition 2018+)

## Installation

Add to your `Cargo.toml`:

```toml
[dependencies]
dbgeng-sys = { git = "https://github.com/your-username/dbgeng-sys" }
```

## Build Notes

Ensure `dbgeng.dll` and `dbghelp.dll` are available.
`build.rs` uses the default path:

```
C:\Program Files (x86)\Windows Kits\10\Debuggers\x64
```
