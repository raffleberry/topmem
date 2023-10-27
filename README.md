# topmem
### Installation
for ubuntu
```sh
sudo apt install python3-pip && pip install --user psutil
```

### options
```sh
$ topmem -h   
usage: topmem [-h] [-g] [-a] [-f]

options:
  -h, --help  show this help message and exit
  -g          group memory usage by application
  -a          view all processes
  -f          print full program path
```

### shows top 10 memory processes
```sh
$ topmem
 1. 1107.87 MB  qbittorrent                   
 2. 644.22 MB   plasmashell                   
 3. 436.50 MB   vlc                           
 4. 364.75 MB   chrome                        
 5. 361.25 MB   dropbox                       
 6. 257.17 MB   chrome                        
 7. 254.93 MB   chrome                        
 8. 244.75 MB   code                          
 9. 240.70 MB   kded5                         
10. 203.48 MB   kwin_x11                      
```

### group all processes by application
```sh
$ topmem -g
 1. 1685.43 MB  (13) chrome                        
 2. 1472.91 MB  (13) code                          
 3. 1107.99 MB  (1) qbittorrent                   
 4. 644.22 MB   (1) plasmashell                   
 5. 438.00 MB   (1) vlc                           
 6. 361.25 MB   (1) dropbox                       
 7. 240.70 MB   (1) kded5                         
 8. 203.60 MB   (1) kwin_x11                      
 9. 154.65 MB   (1) Xorg                          
10. 120.59 MB   (1) polkit-kde-authentication-a...
```

### show full program path
```sh
 1. 1108.37 MB  /usr/bin/qbittorrent          
 2. 644.22 MB   /usr/bin/plasmashell          
 3. 439.13 MB   /usr/bin/vlc                  
 4. 364.70 MB   /opt/google/chrome/chrome     
 5. 361.25 MB   /home/user/.dropbox-dist/dropbox-lnx.x86_64-185.4.6054/dropbox
 6. 258.41 MB   /opt/google/chrome/chrome     
 7. 257.17 MB   /opt/google/chrome/chrome     
 8. 249.54 MB   /usr/share/code/code          
 9. 240.70 MB   /usr/bin/kded5                
10. 203.60 MB   /usr/bin/kwin_x11             
```