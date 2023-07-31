# nextgensay

nextgensay uses `cowsay` and `fortune` to print "Star Trek: The Next Generation" quotes on the terminal. 🖖

## Installation

### Install cowsay and fortune
Arch
```
sudo pacman -S cowsay fortune-mod
sudo ln -sf $PWD/cowsay/* /usr/share/cows/
sudo ln -sf $PWD/fortune/* /usr/share/fortune/
```

Debian
```
sudo apt install cowsay fortune
sudo ln -sf $PWD/cowsay/* /usr/share/cowsay/cows/
sudo ln -sf $PWD/fortune/* /usr/share/games/fortunes/
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

### Message of the Day
The Enterprise D can greet you with a quote on login by adding to `motd`.

Debian  

`sudo vim /etc/update-motd.d/99-footer`

```
#!/bin/sh

exec /usr/games/fortune sttng | /usr/games/cowsay -f enterprised
```


