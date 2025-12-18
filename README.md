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
