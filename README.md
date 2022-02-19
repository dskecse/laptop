[![build](https://github.com/dskecse/laptop/actions/workflows/main.yml/badge.svg)](https://github.com/dskecse/laptop/actions/workflows/main.yml)

# Laptop

Laptop is a script for setting up macOS dev environment.

## Setup

### Prerequisites

Add a symlink to `laptop.local` with customizations before running the main script:

    ln -s ~/.laptop/laptop.local ~/.laptop.local

### Install

Use [laptop script](https://github.com/dskecse/laptop) to set up
a macOS development environment:

    bash <(curl -s https://raw.githubusercontent.com/dskecse/laptop/main/mac) 2>&1 | tee ~/laptop.log
