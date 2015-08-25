# MPlayer motion vector and block type rendering

    mplayer -lavdopts vismv=1:debug=0x4000 ~/simpsons_movie_trailer.mp4
    
![Simpsons Movie](https://github.com/sfvideo/mplayer-debug/blob/master/simpsons.png)

* Red Macroblocks: "I" encoded (You don't need a full "I Frame" to have Inter encoded data)
* Green Macroblocks: "P" encoded (Forward Prediction)
* Purple Macroblocks: "B" encoded (Bi-Directional Prediction)

Arrows represent the motion vectors used to move blocks around.

## References:

* http://libav.org/avconv.html "vismv"
* http://www.ffmpeg.org/ffmpeg-all.html "debug flags"
* http://www.mplayerhq.hu/DOCS/man/en/mplayer.1.html "−lavdopts"
