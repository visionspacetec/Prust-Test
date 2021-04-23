
[![crates.io](https://img.shields.io/crates/v/prust_test.svg)](https://crates.io/crates/prust_test)
[![WIKI](https://img.shields.io/badge/wiki-prust-yellow.svg)](https://github.com/visionspacetec/Prust/wiki)
# Prust-Test
Prust-Test is a tool to send and recieve telecommand and telemetry packets of [PUS-C](https://ecss.nl/standard/ecss-e-st-70-41c-space-engineering-telemetry-and-telecommand-packet-utilization-15-april-2016/) from a command line.

## Usage
After installing, type
```
prust_test
```
Then you will see the list of ports connected.  
Enter your device index from the list when prompted then you may use the CLI!
You can get help by:
```
>> help
```

```
USAGE:
    tc [SUBCOMMAND]

FLAGS:
    -h, --help       Prints help information
    -V, --version    Prints version information

SUBCOMMANDS:
    exec_func       Sends a request to execute a function defined
    help            Prints this message or the help of the given subcommand(s)
    new_report      Creates new housekeeping report structure
    one_shot        Sends a one shot request for the specified hk id
    periodic_dis    Disables peridic report of parameters of the given struct ids
    periodic_en     Enables peridic report of parameters of the given struct ids
    q               quit
```

For more on  ```prust_test``` check the wiki page: [How to Use Prust Test](https://github.com/visionspacetec/Prust/wiki/How-to-Use-Prust-Test).

## Available Telecommands
|Name | Telecommand Description |
|-|-|
|exec_func|     TC[8,1] perform a function|
|new_report|    TC[3,1] create a housekeeping parameter report structure|
|one_shot|     TC[3,27] generate a one shot report for housekeeping parameter report structures|
|periodic_en|      TC[3,5] enable the periodic generation of housekeeping parameter reports|
|periodic_dis|    TC[3,6] disable the periodic generation of housekeeping parameter reports|

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
