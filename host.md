# Hosting a Server

Binaries for the server software are available in its [Github repository](https://github.com/cobweb-gang/cobweb-server), as well as build, install and run instructions. Since clicking is so exhausting, we've put the instructions here as well.

## Build & Install

First, install the Rust toolchain if you haven't already. Run the command below and follow the directions presented to you

`curl https://sh.rustup.rs -sSf | sh`

Once you've installed Rust, clone this repository

`git clone https://github.com/cobweb-gang/cobweb-server`

Move into the repository and compile the code

```
cd cobweb-server
cargo build --release
```

Once you've done this, you can run Cobweb as such:

`target/release/cobweb-server -p password`

You must provide a password via the "-p" flag.

Alternatively, you can move the binary into your $PATH and run it without a directory prefix:

```
mv target/release/cobweb-server /usr/local/bin/cobweb-server
cobweb-server -p password
```
