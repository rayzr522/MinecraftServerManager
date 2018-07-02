# Minecraft Server Manager

> A simple server manager script for Minecraft.

This allows you to start, stop, and control your Minecraft server with a few simple keystrokes, and it's all run in the background via `screen`.

* [Usage](#Usage)
* [Installation](#Installation)

## Usage

```bash
mcsm <start|stop|restart|cmd <command>|console|log|config>
```

### `start`

> Starts the server.

### `stop`

> Stops the server, using the optional delay set in the config before shutting down.

### `restart`

> Stops and then restarts the server.

### `cmd <command>`

> Executes `command` in the server console.

### `console`

> Opens the server console by resuming the `screen` session. *Note: to exit the console, do `C-A D`.*

### `config`

> Opens the config file in whatever editor is defined by the `$VISUAL` environment variable, defaulting to `nano` if none is specified.

### `log`

> Opens the latest log file in `less`.

## Installation

First, make sure you have `screen` installed. For macOS, it comes pre-installed, but for various Linux distros you may need to install it via your package manager. For example, in Arch Linux, it's as simple as `sudo pacman -S screen`.

### Fast method

Just download the script to somewhere in your path (although I'd suggest `/usr/local/bin`):

```bash
curl -fsSL https://cdn.rawgit.com/Rayzr522/MinecraftServerManager/master/mcsm -o /usr/local/bin/mcsm
```

### Easy-update method

In order to be able to easily update MinecraftServerManager, you will need to install `git`. Then, after moving somewhere that you want to install your local copy of MinecraftServerManager, run the following commands:

```bash
git clone https://github.com/Rayzr522/MinecraftServerManager.git
cd MinecraftServerManager
ln -s "$(pwd)"/mcsm /usr/local/bin/mcsm
```

Then, to update MinecraftServerManager in the future, just `cd` into the MinecraftServerManager folder that you cloned from GitHub and run `git pull`.

## Join Me

[![Discord Badge](https://github.com/Rayzr522/ProjectResources/raw/master/RayzrDev/badge-small.png)](https://discord.io/rayzrdevofficial)
