[![build](https://github.com/dskecse/laptop/actions/workflows/main.yml/badge.svg)](https://github.com/dskecse/laptop/actions/workflows/main.yml)

# Laptop

Laptop is a script for setting up macOS dev environment.

## Setup

### Prerequisites

Add a symlink to `laptop.local` with customizations before running the main script:

    ln -s ~/.laptop/laptop.local ~/.laptop.local

### Install

Use [thoughtbot's laptop script](https://github.com/thoughtbot/laptop) to set up
a macOS development environment:

    bash <(curl -s https://raw.githubusercontent.com/thoughtbot/laptop/blob/7b18ef65b9a428cac03da3398bb3d83ce9a4faaf/mac) 2>&1 | tee ~/laptop.log
