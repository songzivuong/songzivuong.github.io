---
layout: post
title: "Reading the Rust Book"
categories: Reading Programming
tags: rust
---

Here are some notes I took while I was reading ["the Rust book"](https://doc.rust-lang.org/book/).

My practice code: [rust-book-code](https://github.com/songzivuong/rust-book-code).

{% include toc %}

## Getting Started

### Installation

Refer to [Install Rust](https://www.rust-lang.org/tools/install).

### Cargo

[Cargo](https://doc.rust-lang.org/cargo/) is Rust’s build system and package manager.

Using Cargo to create a new project named `hello_cargo`:

```
cargo new hello_cargo
```

It will produce a directory `src` with a `main.rs` inside, and a `Cargo.toml` file which is Cargo's configuration file and in the [Tom’s Obvious, Minimal Language](https://github.com/toml-lang/toml) format.

## Example: Guessing Game

There is a trap! If you want to use the `rand` crate, you have to declare `extern crate rand;` at the top.