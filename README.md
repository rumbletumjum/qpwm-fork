# qpwm 

## Features
- Floating only.
- Fullscreen toggle.
- Window centering.
- Mix of mouse and keyboard workflow.
- Focus with cursor.

## Build dependencies
- `xlib` (*usually `libX11`*).
- `gcc` (*for compile*)
- `make` (*for make*)

## Dependency installation
### deb
```fish
sudo apt install gcc make libx11-dev git
```
### Arch
```fish
sudo pacman -Sy gcc make libx11 git
```
### RPM
#### Fedora
```fish
sudo dnf install gcc make libX11-devel git
```
#### OpenSUSE
```fish
sudo zypper install gcc make libX11-devel git
```
## Installation
```fish
git clone https://github.com/ssleert/qpwm.git
cd qpwm
sudo make clean install
```

## Configuration
``make``
Edit ``config.h``.

# Running qpwm
Add to `.xinitrc`:
```fish
exec qpwm
```
If you use ``GDM``, ``SDDM``, ``LightDM`` оr anything other display manager 👤

Add this to `/usr/share/xsessions/qpwm.desktop`:
```desktop
[Desktop Entry]
Name=qpwm
Comment=This session runs qpwm as window manager 
Exec=qpwm
Type=Application
```
## Default Keybindings
**Window Management**
| combo                      | action                 |
| -------------------------- | -----------------------|
| `Mouse`                    | focus under cursor     |
| `win` + `Left Mouse`       | move window            |
| `win` + `Right Mouse`      | resize window          |
| `win` + `f`                | maximize toggle        |
| `win` + `c`                | center window          |
| `win` + `q`                | kill window            |
| `win` + `1-6`              | desktop swap           |
| `win` + `Shift` +`1-6`     | send window to desktop |
| `win` + `return` (*enter*) | open terminal (st)     |
| `ALT` + `TAB`.             | focus cycle            |
# Thanks!
| Person          | Action           |
| --------------- | -----------------|
| xZecora         | some fixes       |
| OpenSky         | screenshots      |
| justleoo        | fix readme       |

## Thanks for code
- [tinywm](http://incise.org/tinywm.html)
- [dwm](https://dwm.suckless.org)
- [2bwm](https://github.com/venam/2bwm)
- [sowm](https://github.com/dylanaraps/sowm)
