# Learning Rust

Notes and examples for learning Rust.

- [Learning Rust](#learning-rust)
  - [Data Types](#data-types)
    - [Scalar](#scalar)
    - [Compound](#compound)
    - [String](#string)
  - [Mutability](#mutability)
    - [Constants](#constants)

## Data Types

```rust
fn main() {
  let a: i32 = 0;
  println!("{}", a);
}
```

### Scalar

> Represents a single value (e.g., 1, 9.a, 'c').

- Integer signed and unsigned: `i8`, `i16`, `i32`, `i64`, `i128`, `isize`, `u8`, `u16`, `u32`, `u64`, `u128`, `usize`.
- Floating-point: `f32`, `f64`.
- Boolean: `bool` (i.e., `true` or `false`).
- Character: `char` (e.g., `'c', 'a', '1').

### Compound

### String

String type is a growable, mutable, UTF-8 encoded type.

> It is provided by STL rather than coded into the core language. Rust only has one string type in the core language, which is _the string slice_ (`&str`).

```rust
fn main() {
  let mut a = String.from("Hello");
  a.push_str(" World");
  println!("{}", a);
}
```

## Mutability

Variables are immutable by default, unless you add `mut` keyword.

```rust
let mut a = 10;
```

### Constants

Constants are values that are bound to a name and are not allowed to change. Moreover, you can use them in _global scope_ unlike `let` variables.

```rust
const MAX: i32 = 10;
```
