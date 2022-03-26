# random-fetch
The goal of this repo is to get a different ASCII_DISTRO on every Terminal start from Neofetch
The distro.txt should be up to date with all default available ascii's in neofetch (State 24.03.2022 - Neofetch 7.1.0)
## How to use
Just add those lines into your .zshrc or .bashrc
```bash
NUM=$(shuf -i 1-230 -n 1)
RDIST=$(awk NR==$NUM /pathToFile/distros.txt)
neofetch --ascii_distro $RDIST
```
