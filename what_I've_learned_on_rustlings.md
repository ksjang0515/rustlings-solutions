# What I've learned from Rustlings

## Why `String::trim` returns `&str` not `String`

## String slice `to_string` vs `to_owned`

Reference

- [`to_string()` vs `to_owned()` for string literals](https://users.rust-lang.org/t/to-string-vs-to-owned-for-string-literals/1441)

## Re-export with `pub use`

- [Re-exporting Names with `pub use` (Rust Doc)](https://doc.rust-lang.org/book/ch07-04-bringing-paths-into-scope-with-the-use-keyword.html#re-exporting-names-with-pub-use)

## Hashmap Entry

Reference

- [map_entry (Rust Clippy)](https://rust-lang.github.io/rust-clippy/master/index.html#map_entry)
- [hash_map::Entry (Rust Doc)](https://doc.rust-lang.org/std/collections/hash_map/enum.Entry.html#method.or_insert)

## nested Option (`Option::flatten`)

Reference

- [Option method.flatten (Rust Doc)](https://doc.rust-lang.org/std/option/enum.Option.html#method.flatten)

## `?` vs `unwrap()`

## Pattern matching `ref` vs `&`

Reference

- [Keyword ref (Rust Doc)](https://doc.rust-lang.org/std/keyword.ref.html)

## Box Polymorphic `dyn ???`

## What each `<T>` mean in `impl<T> Wrapper<T>`

First `<T>` after `impl` implies type `T` will be used for the following block.

`<T>` after `Wrapper` implies we are implementing for type `<T>`.

```Rust
impl<T> Wrapper<T> {
  fn new(value:T) -> Self {}
}

impl Wrapper<i32> {
  fn new(value:i32) -> Self {}
}
```
