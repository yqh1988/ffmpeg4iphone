#the modifications to ffplay are in

IMPORTANT

DO NOT use the ffplay-proj posted in quick links here, follow the directions below.

Use the libs included , compile at your own rick.

The version here has been tested on a 3gs but should work on a 3g.

Finally,

FFPLAY will not compile to the simulator only device 2,21 for now.

Blame that on sdl not us.

THE LATEST VERSION of sdllib will through a bad access exception, the version userd here is very early.



More information here
Thanks to Yonas, theo for all their help.

Here are the results with a xvid movie.

bitrate 1500kbs, resolution dvd, size 6 , streamed from an elgato media server.

http://web.me.com/cannonwc/Site/Photos_5.html#3


FFPLAY is a work in progress some videos play really good

Xvid' and mpeg's seem to play very wel, leaving open the possiblity to use it with such servers such as playon's.

Avi's play but the video/audio is badly out of synch.

Divx don't seem to play at all.

HOWEVER

FFPLAY is just a shell around ffmpeg, ffmpeg has lots of encoding options , generally if ffmpeg can play the file, you can provide the same parameters to ffplay.

Most parms are passed via a var array towards the bottom of ffplay.c




You can get the updated code here. The zip has not been repacked, so if you choice to use the zip file you need to copy the ffplay.c from the svn.

http://99.139.107.194/svn/test/portalServer/ffplay/

the svn passwrd and userid are both test

This information will also be uploaded to the ffmpeg4iphone svn
FFplay is going to remain totally open source.

The enchancements will be jointly hosted and handled by

ffmpeg4iphone google site run by yonas, who's done a great job with ffmpeg.

And

me at mooncatventures.com