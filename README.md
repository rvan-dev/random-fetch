# random-fetch
The goal of this repo is to get a different ASCII_DISTO on every Terminal start from Neofetch

## How to use
Just add those lines into your .zshrc or .bashrc
```bash
NUM=$(shuf -i 1-229 -n 1)
RDIST=$(awk NR==$NUM /pathToFile/distros.txt)
neofetch --ascii_distro $test
```
