[![Build Status](https://travis-ci.com/dskecse/laptop.svg?branch=master)](https://travis-ci.com/dskecse/laptop)

## Setup

### macOS

Use [thoughtbot's laptop script](https://github.com/thoughtbot/laptop) to set up
a macOS development environment:

    bash <(curl -s https://raw.githubusercontent.com/thoughtbot/laptop/master/mac) 2>&1 | tee ~/laptop.log

Add a symlink to `laptop.local` before running the aforementioned script to
install custom packages:

    ln -s ~/.laptop/laptop.local ~/.laptop.local
