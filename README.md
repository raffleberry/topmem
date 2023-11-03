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
 1. 499.45 MB   3282    plasmashell                   
 2. 403.13 MB   4043    chrome                        
 3. 317.52 MB   4789    chrome                        
 4. 282.29 MB   4668    spotify                       
 5. 263.47 MB   4592    spotify                       
 6. 254.33 MB   6402    code                          
 7. 233.71 MB   3229    kded5                         
 8. 227.07 MB   7084    chrome                        
 9. 223.15 MB   4813    chrome                        
10. 219.71 MB   4428    chrome                        
                
```

### group all processes by application
```sh
$ topmem -g  
 1. 2787.98 MB  (19)    chrome                        
 2. 1327.10 MB  (12)    code                          
 3. 1029.84 MB  (7)     spotify                       
 4. 499.45 MB   (1)     plasmashell                   
 5. 233.71 MB   (1)     kded5                         
 6. 197.61 MB   (1)     kwin_x11                      
 7. 139.55 MB   (1)     konsole                       
 8. 126.64 MB   (1)     Xorg                          
 9. 52.50 MB    (3)     python3                       
10. 51.56 MB    (1)     kdeconnectd                   
             
```

### show full program path
```sh
$ topmem -f 
 1. 499.45 MB   3282    /usr/bin/plasmashell          
 2. 403.10 MB   4043    /opt/google/chrome/chrome     
 3. 314.53 MB   4789    /opt/google/chrome/chrome     
 4. 276.99 MB   4668    /usr/share/spotify/spotify    
 5. 275.49 MB   6402    /usr/share/code/code          
 6. 263.47 MB   4592    /usr/share/spotify/spotify    
 7. 233.71 MB   3229    /usr/bin/kded5                
 8. 227.63 MB   7084    /opt/google/chrome/chrome     
 9. 221.46 MB   4813    /opt/google/chrome/chrome     
10. 219.71 MB   4428    /opt/google/chrome/chrome     

```

### show pid of grouped processes
```sh
$ topmem -gp 
 1. 2788.35 MB  (19)    chrome                        
                4043    403.10 MB
                4789    314.53 MB
                7084    227.38 MB
                4813    225.72 MB
                4428    219.71 MB
                4087    184.15 MB
                4484    182.66 MB
                4191    129.49 MB
                4512    128.51 MB
                4088    115.28 MB
                4277    114.00 MB
                7140    104.75 MB
                4212    100.65 MB
                4835    80.62 MB
                9296    67.93 MB
                4060    59.38 MB
                4059    58.75 MB
                4091    55.78 MB
                4064    15.96 MB

 2. 1302.75 MB  (12)    code                          
                6402    235.12 MB
                6655    175.79 MB
                6316    167.79 MB
                6353    165.98 MB
                6610    154.81 MB
                6439    87.70 MB
                6609    80.34 MB
                8942    73.12 MB
                6361    63.34 MB
                6324    44.00 MB
                6323    43.88 MB
                6326    10.88 MB

 3. 1027.43 MB  (7)     spotify                       
                4668    283.53 MB
                4592    263.47 MB
                4613    188.47 MB
                4646    109.32 MB
                4595    73.88 MB
                4596    73.88 MB
                4641    34.89 MB

 4. 499.32 MB   (1)     plasmashell                   
                3282    499.32 MB

 5. 233.71 MB   (1)     kded5                         
                3229    233.71 MB

 6. 197.49 MB   (1)     kwin_x11                      
                3232    197.49 MB

 7. 139.55 MB   (1)     konsole                       
                6113    139.55 MB

 8. 126.64 MB   (1)     Xorg                          
                2888    126.64 MB

 9. 52.50 MB    (3)     python3                       
                705     21.25 MB
                631     18.50 MB
                9374    12.75 MB

10. 51.56 MB    (1)     kdeconnectd                   
                3300    51.56 MB
                    
```

