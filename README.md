# Unsafe Raw Pointer Vector Modification in Rust

This repository demonstrates a potential issue in Rust when modifying a vector using raw pointers.  The example showcases how unsafe operations can lead to unexpected results or program crashes if not carefully managed.  The solution highlights safer alternatives.

## Bug

The `bug.rs` file contains Rust code that modifies a vector's elements using a raw pointer obtained through `as_mut_ptr()`. Although this works in this specific example, it's generally unsafe and can lead to memory corruption or data races.