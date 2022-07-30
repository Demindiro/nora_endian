# Nora endian

[![docs.rs](https://docs.rs/nora_endian/badge.svg)](https://docs.rs/nora_endian)
[![crates.io](https://img.shields.io/crates/v/nora_endian.svg)](https://crates.io/crates/nora_endian)
[![crates.io](https://img.shields.io/crates/d/nora_endian.svg)](https://crates.io/crates/nora_endian)

Yet another crate to deal with endianness, though focused on simplicity

## Example

```rust
use nora_endian::u32le;

let flags = u32le::from(1234);
let index = u32le::from(0);

// Easy operations on & comparisons between le/be and native types
if flags & 1 == 0 {
   // ...
}

let index_plus_one_u32: u32 = 1 + index;
let index_plus_one_u32le: u32le = index + 1;
```
