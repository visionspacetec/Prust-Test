
[![crates.io](https://img.shields.io/crates/v/prust_test.svg)](https://crates.io/crates/prust_test)
[![WIKI](https://img.shields.io/badge/wiki-prust-yellow.svg)](https://github.com/visionspacetec/Prust/wiki)
# Test Tools
Available commands
```
list_ports
```
and 
```
prust_test
```
To see how ```prust_test``` works check the wiki page: [How to Use Prust Test](https://github.com/visionspacetec/Prust/wiki/How-to-Use-Prust-Test).

## Requirements
For GNU Linux pkg-config headers are required:
```
Ubuntu: sudo apt install pkg-config  
Fedora: sudo dnf install pkgconf-pkg-config
```

Libudev headers are needed for gnu linux.
```
Ubuntu: sudo apt install libudev-dev  
Fedora: sudo dnf install systemd-devel
```
For windows some build tools will be required (Will be warned by the OS about that after you try to run the program).
Nightly rust is required.
```
rustup default nightly  
```
## Install
```
cargo install prust_test
```
