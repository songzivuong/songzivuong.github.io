---
layout: post
title: "Reading Programming Rust"
categories: Reading Programming
tags: rust
---

[*Reading Programming: Fast, Safe Systems Development*](http://shop.oreilly.com/product/0636920040385.do) (By Jim Blandy, Jason Orendorff. 2017).

My practice code for this book: [programming-rust-code](https://github.com/songzivuong/programming-rust-code).

{% include toc %}

Systems programming is for:

- Operating systems
- Device drivers of all kinds
- Filesystems
- Databases
- Code that runs in very cheap devices, or devices that must be extremely reliable
- Cryptography
- Media codecs (software for reading and writing audio, video, and image files)
- Media processing (for example, speech recognition or photo editing software)
- Memory management (for example, implementing a garbage collector)
- Text rendering (the conversion of text and fonts into pixels)
- Implementing higher-level programming languages (like JavaScript and Python)
- Networking
- Virtualization and software containers
- Scientific simulations
- Games

In short, systems programming is *resource-constrained* programming.

> Enter Rust: a safe, concurrent language with the performance of C and C++.

The key to promise memory safety and trustworthy concurrency is Rust's system of *ownership*, *moves*, and *borrows*, checked at compile time. 