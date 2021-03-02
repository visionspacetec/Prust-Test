# Test Tools
Available commands
```
cargo run list_ports
```
and 
```
cargo run
```
To see how ```cargo run``` works check the wiki page: [How to Use Prust Test](https://github.com/visionspacetec/Prust/wiki/How-to-Use-Prust-Test).

## Setup
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
