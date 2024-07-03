# Redis and Rust

## A Brief Introduction to Rust

Rust is blazingly fast and memory-efficient: with no runtime or garbage collector, it can power performance-critical services, run on embedded devices, and easily integrate with other languages. Rust’s rich type system and ownership model guarantee memory-safety and thread-safety — enabling you to eliminate many classes of bugs at compile-time.

Rust has great documentation, a friendly compiler with useful error messages, and top-notch tooling — an integrated package manager and build tool, smart multi-editor support with auto-completion and type inspections, an auto-formatter, and more.

- [Getting Started with Rust](https://www.rust-lang.org/learn/get-started)
- [Try Rust without installing](https://play.rust-lang.org/)
- [Rust Tools](https://www.rust-lang.org/tools)

## Using Redis with Rust


## Pre-requisite

- Install Rust on your Mac system

Rust is installed and managed by the rustup tool.

```
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```


## Configure your current shell:
 
```
source $HOME/.cargo/env
```

## Verify Rust compiler:
 
```
rustc --version
rustc 1.49.0
```

- Install Redis

```
docker run --rm -p 6379:6379 redis
```

## Steps 



### Clone the repository

```
git clone https://github.com/redis-developer/rust-redis-101
cd rust-redis-101
```

### Export

If you’re using a local Redis server (e.g. with Docker) over an insecure connection without any password, simply use:

```
export REDIS_HOSTNAME=localhost:6379
```


### Run the application


```
cargo run
```

## Verify the Output


```
   Compiling redis-rust-getting-started v0.1.0 (/Users/ajeetraina/projects/rust-redis-101)
    Finished dev [unoptimized + debuginfo] target(s) in 0.70s
     Running `target/debug/rust-redis-101`
******* Running SET, GET, INCR commands *******
value for 'foo' = bar
counter = 16
```

## Conclusion

Today you learned how to use the Rust driver for Redis to connect and execute operations in Redis.

## Credits

- https://medium.com/swlh/tutorial-getting-started-with-rust-and-redis-69041dd38279
