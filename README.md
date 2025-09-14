# 🍺 Beer v2.0.1 🍺

![cheers](https://media.tenor.com/EcUEfGy--MQAAAAM/getcampedonnerd.gif)

### This provides the Arch Linux package for **Beer**, a command that refuses to serve non-root users, but prints some *root* beer when run with `sudo`.
### I started this project to learn packaging and to continue a joke I made once lol.

![Bash Script](https://img.shields.io/badge/bash_script-%23121011.svg?style=for-the-badge&logo=gnu-bash&logoColor=white) ![Arch](https://img.shields.io/badge/Arch%20Linux-1793D1?logo=arch-linux&logoColor=fff&style=for-the-badge) [![License: GPL v2](https://img.shields.io/badge/License-GPL_v2-blue.svg)](https://www.gnu.org/licenses/old-licenses/gpl-2.0.en.html) 
## Installation

### Prebuilt
[![GitHub release](https://img.shields.io/github/v/release/M0KA907/Beer?sort=semver)](https://github.com/M0KA907/Beer/releases/latest)

Download the latest `.pkg.tar.zst` from the release page, then install it using:
```bash
sudo pacman -U  beer-2.0.1-1-any.pkg.tar.zst 
```
### From Source
```bash
git clone https://github.com/M0KA907/Beer.git
cd Beer
makepkg -si
```
# Usage
```bash
beer        # reserves the right to refuse service to those without root
sudo beer   # Serves user a mug of Root Beer (clears before printing the ASCII)
```
![beer](https://i.imgur.com/05akGUu.png)
![sudo beer](https://i.imgur.com/eQbdx9d.png)
