
# syncpac

A single file executable python script for managing pacman/aur packages across computers with synced user folders, on Arch based Linux distros.

Run `syncpac -h` for help, or `syncpac {command} -h` for help specific to a single command.

## Installation

Syncpac can be ran by invoking the script's path in the command line, so the script can be put anywhere on the user's PATH.

## Setup

Run `syncpac init`, and optionally edit the resulting list of pacman/aur packages.

## Usage

After initializing syncpac, pacman packages that are meant to be synced can be installed with `syncpac install {packages...}` (or `syncpac S {packages...}`). Pacman packages that are meant to be removed from all synced systems can be removed with `syncpac remove {packages...}` (or `syncpac R {packages...}`).
To modify aur packages, use the `--aur` argument.

## Notes

The only aur backend used while developing syncpac has been `yay`, but any aur backend that uses the same syntax as `pacman` may be used with the `--aur-backend {backend}` argument.

I recommend [Syncthing](https://syncthing.net/) for syncing home folders between systems.

No AI was used, consulting included.
