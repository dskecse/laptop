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

Unix tools:

* [Git](https://git-scm.com) for version control
* [Tig](https://jonas.github.io/tig/) for easier browsing of changes in a Git repo and cherry-picking commits
* [OpenSSL](https://www.openssl.org) for Transport Layer Security (TLS)
* [RCM](https://github.com/thoughtbot/rcm) for managing dotfiles
* [Ag](https://github.com/ggreer/the_silver_searcher) (aka "The Silver Searcher") for finding things in files, a faster alternative to `grep` and `ack`
* [Tmux](https://github.com/tmux/tmux/wiki) for saving project state and switching between projects
* [Zsh](https://www.zsh.org) as a default shell
* [Oh My Zsh](https://ohmyz.sh) for managing Zsh configuration
* [watch](https://gitlab.com/procps-ng/procps) for executing a program periodically and showing the output fullscreen
* [duff](https://github.com/elmindreda/duff) for finding duplicate files
* [jq](https://jqlang.org/) for processing JSON
* [yq](https://mikefarah.gitbook.io/yq/) for processing YAML
* [Graphviz](https://www.graphviz.org) for visualizing graphs
* [Nmap](https://nmap.org) for network discovery and security auditing
* [dos2unix](https://waterlan.home.xs4all.nl/dos2unix.html) for converting text between DOS, UNIX, and Mac formats
* [HTTPie](https://httpie.io/) a command-line HTTP and API testing client
* [ShellCheck](https://www.shellcheck.net/) for finding bugs in shell scripts
* [cloc](https://github.com/AlDanial/cloc/) for counting lines of code
* [samply](https://github.com/mstange/samply) a command-line CPU profiler with Firefox Profiler compatible reports
* [Qlty CLI](https://qlty.sh) (ex-CodeClimate) for automating code quality checks, linting and auto-formatting code

Terminal:

* [iTerm2](https://iterm2.com) a replacement for default macOS Terminal
* TODO: Try out [Ghostty](https://ghostty.org) or [Warp](https://www.warp.dev/mac-terminal)

GitHub tools:

* [GitHub CLI](https://cli.github.com) for interacting with the GitHub API
* [gist](https://defunkt.io/gist/) for uploading Gists

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

Programming languages, package managers and prerequisites:

* [jemalloc](https://jemalloc.net) a general purpose `malloc(3)` implementation that emphasizes fragmentation avoidance and scalable concurrency support
* [LibYAML](https://github.com/yaml/libyaml) for parsing and emitting YAML, external Ruby dependency
* [Coreutils](https://www.gnu.org/software/coreutils/) for basic file, shell and text manipulation utilities expected to exist on every operating system, see [more info](https://www.maizure.org/projects/decoded-gnu-coreutils/)
* [Readline](https://tiswww.case.edu/php/chet/readline/rltop.html) for maintaining a list of previously-entered command lines, recalling and reediting those lines, external Ruby dependency
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

Media tools:

* [Cyberduck](https://cyberduck.io) for uploading media files to S3 buckets and browsing cloud storage
* [LAME](https://lame.sourceforge.io) for encoding MPEG Audio Layer III (MP3)
* [FFmpeg](https://ffmpeg.org) for recording, converting and streaming audio and video
* [ExifTool](https://exiftool.org) for reading and writing EXIF metadata
* [HandBrake](https://handbrake.fr) for converting video from nearly any format to a selection of modern, widely supported codecs
* [IINA](https://iina.io) a modern media player for macOS

Browsers and related tools:

* [Firefox](https://www.firefox.com/en-US/)
* [ChromeDriver](https://developer.chrome.com/docs/chromedriver/) for automated testing of webapps using Google Chrome

Containers & orchestration tools:

* [OrbStack](https://orbstack.dev) for faster, lighter, and easier way to run Docker containers, a replacement for Docker Desktop
* [Kubernetes CLI](https://kubernetes.io/docs/reference/kubectl/) for communicating with a Kubernetes cluster's control plane, using the Kubernetes API
* [kind](https://kind.sigs.k8s.io/) for running local Kubernetes clusters using Docker
* [Helm](https://helm.sh/) for managing Kubernetes packages and apps

Cloud management tools:

* [gcloud CLI](https://cloud.google.com/cli) for managing resources and applications hosted on Google Cloud
* [Hashicorp Vault](https://github.com/hashicorp/vault) for managing secrets and protecting sensitive data

OpenPGP encryption & signing tools:

* [GPG2](https://gnupg.org) for encrypting and signing data, e.g. Git commits, see [more info](https://docs.releng.linuxfoundation.org/en/latest/gpg.html)
* [pinentry-mac](https://github.com/GPGTools/pinentry) for entering PINs or GPG passphrases in a native-looking pop-up window and preventing them from being logged, see [more info](http://support.gpgtools.org/discussions/problems/42548-passphrase-window-not-shown)
* [Keychain](https://www.funtoo.org/Funtoo:Keychain) for launching only one instance of a GPG agent and sharing the agent across every shell, see [more info](https://nullprogram.com/blog/2012/06/08/)

VPNs:

* [TunnelBear VPN](https://www.tunnelbear.com)
* [OpenVPN Connect](https://openvpn.net/client/) for accessing organization's network resources securely

Misc:

* [Dropbox](https://www.dropbox.com/)
* [ngrok](https://ngrok.com/) for exposing APIs online
* [Fliqlo](https://fliqlo.com/) a flip clock screensaver
