This project will patch ffmpeg so you can compile and run ffmpeg, ffplay, and ffserver on the iPhone and iPod Touch.

The initial patch is based on http://svn.telesphoreo.org/trunk/data/ffmpeg_

I have compiled ffmpeg with the following options:

--disable-shared --enable-static --disable-vhook --disable-mmx --disable-iwmmxt --disable-armvfp --enable-libfaad --enable-gpl --enable-libvorbis --enable-libfaac --enable-libtheora --enable-libx264 --enable-libxvid --enable-libmp3lame --enable-postproc --disable-armv5te --enable-armv6 --disable-debug --disable-stripping --enable-swscale --enable-avfilter --enable-avfilter-lavf --arch=arm


<br><br>

<hr>

<br>
<b>Good news!</b>

There seems to be a better way to compile FFmpeg for the iPhone, and it doesn't include any patching!<br>
<br>
<a href='http://lists.mplayerhq.hu/pipermail/ffmpeg-devel/2009-October/076618.html'>gas-preprocesor</a>
<br>
<br>
<hr><br>
<br>
<br>
<br>
<br>
<b>IMPORTANT MESSAGE:</b>
Please do not request specific files or recompiling with different options. All the source code is freely available.<br>
<br>
<br>

<b>Minimum Requirements:</b>
<br>
<br>
<hr><br>
<br>
<br>
<br>
<ul>
<li>Firmware 2.1 or later</li>
</ul>

<br>
<b>Cydia:</b>
<br>
<br>
<hr><br>
<br>
<br>
To install ffmpeg in Cydia, add the <a href='http://apt.modmyi.com'>ModMyi repository</a>.<br>
<br>
<br>
<b>Manual Installation Instructions:</b>
<br>
<br>
<hr><br>
<br>
<br>
<br>
<ol>
<li>Download ffmpeg from the Downloads section and copy it to your device</li>
<li>Set permissions: chmod 755 ffmpeg</li>
<li>Run ffmpeg: ./ffmpeg</li>
</ol>

These steps can be used to run ffserver, as well.<br>
<br>
<br>
<b>Documentation:</b>
<br>
<br>
<hr><br>
<br>
<br>
<a href='http://ffmpeg.org/ffmpeg-doc.html#SEC2'>FFmpeg.org</a>