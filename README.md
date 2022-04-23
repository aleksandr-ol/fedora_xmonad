# fedora_xmonad
xorg  
startx  
  
# set resolution  
xrandr  
cvt 1920 1080  
xrandr --setmode  
xrandr --output Virtual-1 --mode "1920x1080_60.00"  

OR  
/etc/X11/xorg.conf.d/10-monitor.conf  

```Section "Monitor"
### Monitor Identity - Typically HDMI-0 or DisplayPort-0
    Identifier    "HDMI1" 

### Setting Resolution and Modes
## Modeline is usually not required, but you can force resolution with it    
Modeline "1920x1080" 172.80 1920 2040 2248 2576 1080 1081 1084 1118
    Option "PreferredMode" "1920x1080"
    Option        "TargetRefresh" "60"

### Positioning the Monitor
## Basic
    Option "LeftOf or RightOf or Above or Below" "DisplayPort-0"    
## Advanced
    Option        "Position" "1680 0"

## Disable a Monitor
     Option        "Disable" "true"
EndSection ```

# haskell compile error
"gcc: error: /usr/lib/rpm/redhat/redhat-hardened-cc1: No such file or directory" CentOS's and Fedora +22 workaround  
Install `redhat-rpm-config`  
$ sudo dnf install redhat-rpm-config  
