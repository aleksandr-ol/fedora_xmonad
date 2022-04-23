# fedora_xmonad
xorg  
startx  
  
# set resolution  
xrandr  
cvt 1920 1080  
xrandr --setmode  
xrandr --output Virtual-1 --mode "1920x1080_60.00"  

# haskell compile error
"gcc: error: /usr/lib/rpm/redhat/redhat-hardened-cc1: No such file or directory" CentOS's and Fedora +22 workaround  
Install `redhat-rpm-config`  
$ sudo dnf install redhat-rpm-config  
