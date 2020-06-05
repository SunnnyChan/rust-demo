Rust Develop Demo
=================

# Get Start 

```bash
# 创建工程项目
$cargo new rust-demo
     Created binary (application) `rust-demo` package

$tree get-start/
get-start/
├── Cargo.toml
└── src
    └── main.rs

$cat get-start/src/main.rs
fn main() {
    println!("Hello, world!");
}

$cat get-start/Cargo.toml
[package]
name = "get-start"
version = "0.1.0"
authors = ["sunnychan <sunnnychan@gmail.com>"]
edition = "2018"

# See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html

[dependencies]

# 使用 Cargo 构建程序
$cargo build
   Compiling get-start v0.1.0 (/Users/sunny/WorkPlace/demo/rust/rust-demo/get-start)
    Finished dev [unoptimized + debuginfo] target(s) in 0.39s

$tree get-start/
get-start/
├── Cargo.lock
├── Cargo.toml
├── src
│   └── main.rs
└── target
    └── debug
        ├── build
        ├── deps
        │   ├── get_start-c13610cfc1f55c78
        │   ├── get_start-c13610cfc1f55c78.d
        │   └── get_start-c13610cfc1f55c78.dSYM
        │       └── Contents
        │           ├── Info.plist
        │           └── Resources
        │               └── DWARF
        │                   └── get_start-c13610cfc1f55c78
        ├── examples
        ├── get-start
        ├── get-start.d
        ├── get-start.dSYM -> deps/get_start-c13610cfc1f55c78.dSYM
        └── incremental
            └── get_start-fql6es6wh6bc
                ├── s-fo2wl97yls-n6k7rr-2l8h3shwozd0y
                │   ├── 1ludobs8mrs38hmm.o
                │   ├── 2vdnr96691v4iat8.o
                │   ├── 31v2vi7pzr0x93ip.o
                │   ├── 3i8aoeuw62hggm5a.o
                │   ├── 3z3llm367hz0rh8.o
                │   ├── dep-graph.bin
                │   ├── query-cache.bin
                │   ├── rhvnsfp6lqptlfv.o
                │   └── work-products.bin
                └── s-fo2wl97yls-n6k7rr.lock

14 directories, 20 files

# 使用 Cargo 运行程序
$cargo run
    Finished dev [unoptimized + debuginfo] target(s) in 0.00s
     Running `target/debug/get-start`
Hello, world!

# 直接运行二进制文件

$./target/debug/get-start
Hello, world!

$cargo clean

$tree get-start/
get-start/
├── Cargo.lock
├── Cargo.toml
└── src
    └── main.rs

```

