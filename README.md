# Aaron's build of dwm

### Patches
- [actualfullscreen](https://dwm.suckless.org/patches/actualfullscreen/)
- [alwayscenter](https://dwm.suckless.org/patches/alwayscenter/)
- [moveresize](https://dwm.suckless.org/patches/moveresize/)
- [notitle](https://dwm.suckless.org/patches/notitle/)
- [pertag](https://dwm.suckless.org/patches/pertag/)
- [swallow](https://dwm.suckless.org/patches/swallow/)
- [switchtotag](https://dwm.suckless.org/patches/switchtotag/)
- [fibonacci](https://dwm.suckless.org/patches/fibonacci/)
- [smartborders](https://dwm.suckless.org/patches/smartborders/)
- [tilegap](https://dwm.suckless.org/patches/tilegap/)

### Install
```bash
git clone https://git.sr.ht/~unrealapex/dwm
cd dwm
sudo make clean install
```

### Setup
`~/.xinitrc`:
```bash
feh --bg-fill <aesthetic-wallpaper>

while true; do
   xsetroot -name "$( date +"%m/%d %I:%M %P" )"
   sleep 1
done &

while true; do
    # Log stderror to a file 
    dwm 2> ~/.dwm.log
    # No error logging
    #dwm >/dev/null 2>&1
done
```

