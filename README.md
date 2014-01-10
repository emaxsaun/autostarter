Autostarter
==========

About this Plugin:

This is a small JW Player Plugin if you want a video on your site to automatically start the first X times a user visits your website. The plugin drops this history in a cookie, so after the Xth time the video won't autostart. Great for promos you want your users to see.

Configuration Options:

This plugin supports additional configuration options via flashvars. You can read about the available options below and see examples below.

Flashvar: autostarter.count = This is the number of times to autostart the video for before it will no longer autostart.

Implementing this Plugin:

There is one file that you need to use, autostarter.js. Upload this file to your server, it can go anywhere on the server. Now, inside of your JW Player embed code, make sure that your plugins call points to the full path to the .js file on your server (http://www.yoursite.com/autostarter.js).

Example (stops autostarting after 5 times):

<pre>
&lt;script type=&quot;text/javascript&quot; src=&quot;jwplayer.js&quot;&gt;&lt;/script&gt;
&lt;div id=&quot;player&quot;&gt;&lt;/div&gt;
&lt;script type=&quot;text/javascript&quot;&gt;
jwplayer('player').setup({
&nbsp;&nbsp;'width': '575',
&nbsp;&nbsp;'height': '400',
&nbsp;&nbsp;'file': 'video.mp4'
&nbsp;&nbsp;'image': &quot;video.jpg&quot;,
&nbsp;&nbsp;plugins: {
	&nbsp;&nbsp;&nbsp;&nbsp;&quot;autostarter.js&quot;: {
	&nbsp;&nbsp;&nbsp;&nbsp;'count':'5'
	&nbsp;&nbsp;}
&nbsp;&nbsp;}
});
&lt;/script&gt;
</pre>

The source code is available for this plugin. There is just a .js file for JavaScript. Publishing the JavaScipt can be simply done with any text editor. Enjoy~! :) 
