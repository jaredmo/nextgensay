# nextgensay

nextgensay uses `cowsay` and `fortune` to print Star Trek TNG quotes on the command line.

## Installation

### Install cowsay and fortune
Arch
```
sudo pacman -S cowsay fortune-mod
ln -sf $PWD/cowsay/* /usr/share/cows/
ln -sf $PWD/fortune/* /usr/share/fortune/
```

Debian
```
sudo apt install cowsay fortune
ln -sf $PWD/cowsay/* /usr/share/cowsay/cows/
ln -sf $PWD/fortune/* /usr/share/games/fortunes/
```

## Usage
`fortune sttng | cowsay -f enterprised`

```
 _________________________________________ 
/ If there's nothing wrong with           \
| me...maybe there's something wrong with |
| the universe!                           |
|                                         |
\ -- Beverly Crusher, "Remember Me"       /
 ----------------------------------------- 
    \
     \
      \
                _____.-----._____
   ___----~~~~~~. ... ..... ... .~~~~~~----___
=================================================
   ~~~-----......._____________.......-----~~~
    (____)             |   /          (____)
      ||           _/   |   _           ||
       \_______--~  //~~~\  ~--_______//
        `~~~~---__   \___//   __---~~~~'
                  ~~-_______-~~
```
