#### Video Player Example

###### Prerequisite
1. ffmpeg
1. video.js


###### How to convert mp4 to hls?

You need to get `ffmpeg` first
```
ffmpeg -i source.mp4 -codec:v libx264 -codec:a aac -map 0 -f ssegment -segment_format mpegts -segment_list playlist.m3u8 -segment_time 10 north%03d.ts
```

##### How to lauch example

http://localhost:10080/player.html