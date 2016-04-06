<b>
Good news!<br>
<br>
There seems to be a better way to compile FFmpeg for the iPhone, and it doesn't include any patching!<br>
<br>
</b>
[gas-preprocesor](http://lists.mplayerhq.hu/pipermail/ffmpeg-devel/2009-October/076618.html)

<br><br>
<br>
<br>
<hr><br>
<br>
<br>
<br>
<h1>Build Instructions</h1>

<ol>
<li> On the iPhone/iPod Touch, install ldid from Cydia </li>
<li> Download and install iPhone SDK >= 2.1 for Mac OS X</li>
<li> In Mac OS X, download ffmpeg from svn (replace -<a href='https://code.google.com/p/ffmpeg4iphone/source/detail?r=20161'>r20161</a> with the revision you want)<br>
<br>
<pre><code>svn checkout svn://svn.ffmpeg.org/ffmpeg/trunk -r20161 ffmpeg<br>
</code></pre>

<b>NOTE:</b>  Changes in libswscale are now causing compiler problems for ffmpeg4iphone <= 0.0.4.x. Please use ffmpeg4iphone-0.0.6 or later.<br>
<br>
<br>
Unknown end tag for </li><br>
<br>
<br>
<li> Use a configure script from the Download section</li>

<pre><code>cd ffmpeg<br>
patch -p4 -i ffmpeg4iphone-svn-2009-10-03-v0.0.6.patch<br>
./configure-iphone-v0.0.5<br>
</code></pre>
<li>Copy ffmpeg to the iPhone/iPod Touch</li>

<li>On the iPhone/iPod Touch, run: ldid -S ffmpeg</li>
<br>
<br>
Unknown end tag for </ol><br>
<br>
<br>
<br>
<h1>Configuring and compiling other plugins</h1>
Use the configure files at:<br>
<a href='http://code.google.com/p/ffmpeg4iphone/issues/detail?id=1&can=1'>http://code.google.com/p/ffmpeg4iphone/issues/detail?id=1&amp;can=1</a>

You can use those ones configure files as a good template for configuring other plugins. The only thing you would usually need to change is the actual ./configure line in the file.