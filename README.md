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
ffmpeg -i input.mp4 -vf fps=10,scale=300:-1:flags=lanczos output.gif
```

```
ffmpeg -i input.mp4 -r 10 -an -ss '00:11:02.5' -to '00:11:05' output.gif
```

#### video conver
Constant Rate Factor (CRF)
```
ffmpeg -i input.mp4 -c:v libx264 -crf 22 -c:a copy output.mp4
```


Lossless
Fast encoding example:
```
ffmpeg -i input -c:v libx264 -preset ultrafast -qp 0 output.mkv
```
Best compression example:
```
ffmpeg -i input -c:v libx264 -preset veryslow -qp 0 output.mkv
```

https://trac.ffmpeg.org/wiki/Encode/H.264

#### help
```
tldr tldr
```
