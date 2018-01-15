# Minecraft Server Manager

> A simple server manager script for Minecraft.

This allows you to start, stop, and control your Minecraft server with a few simple keystrokes, and it's all run in the background via `screen`.

## Installation

Just download the script to somewhere in your path (although I'd suggest `/usr/local/bin`):

```bash
curl -fsSL https://cdn.rawgit.com/Rayzr522/MinecraftServerManager/master/mcsm -o /usr/local/bin/mcsm
```

Then make sure you have `screen` installed. For macOS, it comes pre-installed, but for various Linux distros you may need to install it via your package manage. For Arch Linux, it's as simple as `sudo pacman -S screen`.

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

## Join Me

[![Discord Badge](https://github.com/Rayzr522/ProjectResources/raw/master/RayzrDev/badge-small.png)](https://discord.io/rayzrdevofficial)