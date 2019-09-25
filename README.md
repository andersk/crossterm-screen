![Lines of Code][s7] [![Latest Version][s1]][l1] [![MIT][s2]][l2] [![docs][s3]][l3] [![Join us on Discord][s5]][l5]

# Crossterm Screen

This crate allows you to work with alternate and raw screen cross-platform. 
It supports all UNIX and windows terminals down to windows 7 (not all terminals are tested
see [Tested Terminals](#tested-terminals) for more info)

This crate is a sub-crate of [crossterm](https://crates.io/crates/crossterm) to move between screen
buffers and switch to raw-mode, it can be use individually.

Other sub-crates are:

- [crossterm_style](https://crates.io/crates/crossterm_style) 
- [crossterm_terminal](https://crates.io/crates/crossterm_terminal) 
- [crossterm_input](https://crates.io/crates/crossterm_input)
- [crossterm_cursor](https://crates.io/crates/crossterm_cursor)
 
When you want to use other modules as well you might want to use crossterm with
[feature flags](https://crossterm-rs.github.io/crossterm/docs/feature_flags.html).
 
In case you are wondering what 'alternate' or 'raw' screen is, you could checkout the
[book](https://crossterm-rs.github.io/crossterm/docs/screen.html) describing this in more detail.
  
## Table of contents:

- [Getting started](#getting-started)
- [Useful links](#useful-links)
- [Features](#features)
- [Examples](#examples)
- [Tested Terminals](#tested-terminals)
- [Authors](#authors)
- [License](#license)

## Getting Started

All examples of how `crossterm_input` works can be found in the [examples](https://github.com/crossterm-rs/examples)
repository. You might consider reading the [book](https://crossterm-rs.github.io/crossterm/docs/screen.html) which
has a dedicated section on alternate and raw modes.

Add the `crossterm_screen` package to your `Cargo.toml` file.

```
[dependencies]
crossterm_screen = "0.3"
```

And import the `crossterm_screen` modules you want to use.

```rust  
pub use crossterm_screen::{AlternateScreen, RawScreen};
```

### Useful Links

- [Documentation](https://docs.rs/crossterm_screen/)
- [Crates.io](https://crates.io/crates/crossterm_screen)
- [Book](https://crossterm-rs.github.io/crossterm/docs/screen.html)
- [Examples](https://github.com/crossterm-rs/examples)

## Features

These are the features of this crate:

- Cross-platform
- Multi-threaded (send, sync)
- Detailed Documentation
- Few Dependencies
- Alternate screen
- Raw screen   
    
Planned features:
- make is possible to switch between multiple buffers.

## Examples

The [examples](https://github.com/crossterm-rs/examples) repository has more complete and verbose examples.

## Tested terminals

- Windows Powershell
    - Windows 10 (pro)
- Windows CMD
    - Windows 10 (pro)
    - Windows 8.1 (N)
- Ubuntu Desktop Terminal
    - Ubuntu 17.10
- (Arch, Manjaro) KDE Konsole
- Linux Mint

This crate supports all Unix terminals and windows terminals down to Windows 7 but not all of them have been tested.
If you have used this library for a terminal other than the above list without issues feel free to add it to
the above list, I really would appreciate it.

## Authors

* **Timon Post** - *Project Owner & creator*

## License

This project is licensed under the MIT License - see the [LICENSE.md](./LICENSE) file for details

[s1]: https://img.shields.io/crates/v/crossterm_screen.svg
[l1]: https://crates.io/crates/crossterm_screen

[s2]: https://img.shields.io/badge/license-MIT-blue.svg
[l2]: ./LICENSE

[s3]: https://docs.rs/crossterm_screen/badge.svg
[l3]: https://docs.rs/crossterm_screen/

[s5]: https://img.shields.io/discord/560857607196377088.svg?logo=discord
[l5]: https://discord.gg/K4nyTDB

[s7]: https://travis-ci.org/crossterm-rs/crossterm.svg?branch=master
