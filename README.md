# random-fetch
Neofetch, get random ASCII_Distro on every launch of ther Terminal

Tot get a random ascii from the Neofetch given Distros just add those lines into your .zshrc or .bashrc
```bash
NUM=$(shuf -i 1-229 -n 1)
RDIST=$(awk NR==$NUM /pathToFile/distros.txt)
neofetch --ascii_distro $test
```