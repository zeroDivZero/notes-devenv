# `xcode-select`

Manages active developer directory for Xcode and BSD tools.

Allows switching among different Xcode versions and toolchains (e.g., `xcodebuild`), including BSD development commands (such as `cc` and `make`).

Also commonly used to install Xcode command-line tools.

## Install Xcode Command-Line Tools

```sh
xcode-select --install
```

Provides essential utilities like `git`, `clang`, and `make`.

## Select Active Developer Directory

```sh
xcode-select --switch path/to/Xcode.app/Contents/Developer
```

Vital when working with multiple Xcode versions, useful when development and testing require different versions of tools.

`-s` option shorthand.

## Select Xcode Instance and Use Its Developer Directory as Active

```sh
xcode-select --switch path/to/Xcode_file.app
```

When dealing with project-specific requirements or when testing software on different SDKs.

## Print Current Active Developer Directory

```sh
xcode-select --print-path
```

`-p` option shorthand.

## Reset Active Developer Directory

```sh
xcode-select --reset
```

Discard user specification and reset to default.

`-r` option shorthand.
