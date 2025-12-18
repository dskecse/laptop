[![build](https://github.com/dskecse/laptop/actions/workflows/main.yml/badge.svg)](https://github.com/dskecse/laptop/actions/workflows/main.yml)

# Laptop

Laptop is a script for setting up macOS dev environment.

## Setup

Set up macOS dev environment by running the following command:

```sh
sh <(curl -s https://raw.githubusercontent.com/dskecse/laptop/main/mac) 2>&1 | tee ~/laptop.log
```

## Debugging

The above mentioned command's last run will be saved to `~/laptop.log`.
Read through it if there's a need to debug the issue yourself.
If that's not feasible for some reason, feel free to open up a new GitHub issue and attach the whole log file.

## What it sets up

macOS tools:

* [Rosetta 2](https://developer.apple.com/documentation/apple-silicon/about-the-rosetta-translation-environment) for running apps that contain `x86_64` instructions on Apple Silicon processors
* [Homebrew](https://brew.sh) for managing packages on macOS
* [Xcode Command Line Tools](https://developer.apple.com/download/all/?q=Command%20Line%20Tools) for installing compilers, build tools, and Unix utilities necessary for software development on macOS, e.g. Apple LLVM compiler (`clang`), linker, and Make

GitHub tools:

* [GitHub CLI](https://cli.github.com) for interacting with the GitHub API

Editors:

* [Vim](https://www.vim.org)
* [Universal Ctags](https://ctags.io) for indexing files for vim tab completion and locating indexed items

Databases:

* [Postgres 18](https://www.postgresql.org) for storing relational data
* [Redis 8](https://redis.io) for storing key-value data
* [MongoDB 8](https://www.mongodb.com) for storing document-oriented data

Database clients:

* [Postico 2](https://eggerapps.at/postico2/) for managing Postgres databases

Image tools:

* [ImageMagick](https://imagemagick.org) for cropping and resizing images

Programming languages and package managers:

* [Ruby](https://www.ruby-lang.org/en/) latest for writing general-purpose code
* [ruby-install](https://github.com/postmodern/ruby-install) for installing Ruby
* [chruby](https://github.com/postmodern/chruby) for changing the current Ruby
* [Node.js](http://nodejs.org) and [npm](https://www.npmjs.com) for running JavaScript apps and installing JavaScript packages
* [Yarn](https://yarnpkg.com) for managing JavaScript packages
* [Python 3.14](https://www.python.org)
* [Go](https://go.dev)
* [OpenJDK](https://openjdk.org) for compiling Clojure apps to JVM bytecode and running it
* [Clojure](https://clojure.org)
* [Leiningen](https://leiningen.org) for managing Clojure projects and dependencies
* [Haskell](https://www.haskell.org)
* [Cabal](https://cabal.readthedocs.io/en/stable/) for managing Haskell projects and dependencies
* [Wasmtime](https://wasmtime.dev) for running WebAssembly (Wasm) code, see [more info](https://docs.wasmtime.dev)

OpenPGP encryption & signing tools:

* [GPG2](https://gnupg.org) for encrypting and signing data, e.g. Git commits, see [more info](https://docs.releng.linuxfoundation.org/en/latest/gpg.html)
* [pinentry-mac](https://github.com/GPGTools/pinentry) for entering PINs or GPG passphrases in a native-looking pop-up window and preventing them from being logged, see [more info](http://support.gpgtools.org/discussions/problems/42548-passphrase-window-not-shown)
* [Keychain](https://www.funtoo.org/Funtoo:Keychain) for launching only one instance of a GPG agent and sharing the agent across every shell, see [more info](https://nullprogram.com/blog/2012/06/08/)

TBA
