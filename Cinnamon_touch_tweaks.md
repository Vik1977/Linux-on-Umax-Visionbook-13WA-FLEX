 ## Maybe finally i found something that can work like i want it: __Cinnamon__,   
installing Touchegg, Onboard, x11-xserver-utils  

```bash
sudo apt install touchegg onboard x11-xserver-utilis
```

## 1)Screen rotation

Rotate with xrandr:
``` bash
xrandr --output eDP-1 --rotate left
```

You can make a script rotate.sh and bind it to a shortcut:

```bash
#!/bin/bash
xrandr --output eDP-1 --rotate left
```

## 2)On-screen keyboard: Oboard

Enable it at startup:  
Menu → Startup Applications → Add → Onboard.  


## 3)Touch gestures

Then configure gestures in ~/.config/touchegg/touchegg.conf, e.g.:

```bash
<gesture type="SWIPE" fingers="3" direction="UP">
  <action type="COMMAND">cinnamon-menu</action>
</gesture>
```
That gives you 3-finger swipe up = open menu.


## 4) Larger UI elements

Make Cinnamon UI more touch-friendly:
```bash
gsettings set org.cinnamon.desktop.interface text-scaling-factor 1.25
gsettings set org.cinnamon.desktop.interface cursor-size 32
```

Also in Cinnamon Settings → Themes, pick a theme with bigger buttons (Mint-Y-Dark with 150% scaling works well).
```bash
sudo apt install mint-y-icons
```

## 5)Trackpad and Tap tweaks

Enable tap-to-click and gestures with:
```bash
gsettings set org.cinnamon.settings-daemon.peripherals.touchpad tap-to-click true
gsettings set org.cinnamon.settings-daemon.peripherals.touchpad natural-scroll true
```

## 6)tablet mode toggle

Create a script tablet-mode.sh:
```bash
#!/bin/bash
# Rotate + launch Onboard + adjust scaling
xrandr --output eDP-1 --rotate left
onboard &
gsettings set org.cinnamon.desktop.interface text-scaling-factor 1.5
```

Make it executable

Bind it to a shortcut in Cinnamon (System Settings → Keyboard → Shortcuts).

