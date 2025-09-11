# Beer v2.0.1 🍺
![cheers](https://media.tenor.com/EcUEfGy--MQAAAAM/getcampedonnerd.gif)
![cheers](https://media.tenor.com/EcUEfGy--MQAAAAM/getcampedonnerd.gif)

This provides the Arch Linux package for **Beer** — a command that refuses to serve non-root users, but prints some *root* beer when run with `sudo`.

## Installation

### Prebuilt
[![GitHub release](https://img.shields.io/github/v/release/DawnStar907/Beer?sort=semver)](https://github.com/DawnStar907/Beer/releases/latest)

Download the latest `.pkg.tar.zst` from the release page, then install it using:
```bash
sudo pacman -U  beer-2.0.1-1-any.pkg.tar.zst 
```
### From Source
```bash
git clone https://github.com/DawnStar907/Beer.git
cd Beer
makepkg -si
```
