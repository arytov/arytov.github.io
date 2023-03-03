# arytov.github.io


#### RAM Memory info
```
sudo dmidecode --type 17
```

#### Mounts file systems
```
cat /proc/mounts
```

#### ssd temp
```
sudo nvme smart-log /dev/nvme0 
```

#### video to gif
```
ffmpeg -i input.mp4 -r 10 -an -ss '00:11:02.5' -to '00:11:05' output.gif
```
