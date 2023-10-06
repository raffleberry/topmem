# topmem
### Installation
for ubuntu
```
sudo apt install python3-pip && pip install --user psutil
```

### options
```
$ topmem -h   
usage: topmem [-h] [-g] [-a]

options:
  -h, --help  show this help message and exit
  -g          group memory usage by application
  -a          view all processes
```

### shows top 10 memory processes
```
$ topmem
1. /opt/google/chrome/chrome (373.16 MB)
2. /usr/bin/gnome-shell (328.55 MB)
3. io.elementary.appcenter (294.79 MB)
4. /opt/google/chrome/chrome (219.22 MB)
5. /opt/google/chrome/chrome (203.78 MB)
6. /usr/share/code/code (199.34 MB)
7. /usr/share/code/code (185.43 MB)
8. /opt/google/chrome/chrome (180.11 MB)
9. /usr/bin/python3 (169.36 MB)
10. /usr/share/code/code (158.71 MB)
```

### group all processes by application
```
$ topmem -g
1. /opt/google/chrome/chrome (2366.23 MB)
2. /usr/share/code/code (1217.83 MB)
3. /usr/bin/plasmashell (402.47 MB)
4. /usr/bin/kded5 (228.18 MB)
5. /usr/bin/kwin_x11 (177.32 MB)
6. /usr/bin/dolphin (159.38 MB)
7. /usr/lib/xorg/Xorg (154.07 MB)
8. /usr/bin/ark (141.75 MB)
9. /lib/systemd/systemd-udevd (141.12 MB)
10. /usr/bin/konsole (125.22 MB)
```