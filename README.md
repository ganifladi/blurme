# blurme

<p>blurme v1.0 Codename MEH (My Eyes Hurt) is a small script which will blur your feh set background if any window, or rofi is open. Furthermore there are some switches wich can be found, when calling 'blurme -h'. It allows setting a custom directory (-d), adding (-a) a new program, which will start the transition, setting the transition time (-t), and finally one which will draw some output (-v) to the commandline.</p>
<p>Please feel free to fork it, make pull requests and use it in your own projects.</p>
<p>This is my first project i publish. Please be gentle on me :)</p>
<h2>How to start</h2>
<h3>Requirements</h3>
<ol>
<li><b>wmctrl</b>: This script makes use of wmctrl to get the current workspace number and to clarify, whether any window is open. It's essential!</li>
<li><b>feh</b>: Furthermore you'll need feh to set your background image(s).</li>
<li><b>imagemagick</b>: And last but not least imagemagick is mandatory to blur the images</li>
</ol>
<h3>Download and ...</h3>
<ol>
    <li>Place it anywhere you like (e.g. ~/.scripts)</li>
    <li>Make it executable (chmod +x ~/.scripts/blurme)</li>
</ol>
<h2>How to run it</h2>
<h3>Manual start</h3>
<p>Run it once in a terminal of your choice with ~/.scripts/blurme</p>
<h3>Autostart</h3>
<h4>i3</h4>
<p>Add the line "exec --no-startup-id ~/.scripts/blurme &" to your i3 config.</p>
<h4>bspwm</h4>
<h4>openbox</h4>
<h3>Options</h3>
<h4>I need more!</h4>
<p>To ddd another program, which will start the blur effect use the script like this:</p>
<p><pre>~/.script/blurme -a rofi</pre></p>
<h4>Custom working dir</h4>
<p>The default working directory is set to <pre>~/.cache/blurme</pre>. If this bothers you for some reason (maybe you have connected this specific directory to your tmpfs), don't worry. You can simply apply another directory to the script with the option <pre>-d</pre></p>
<p><pre>~/.scripts/blurme -d ~/.my/dream/directory</pre></p>
<h4>Custom transition time</h4>
<p>The transition time is measured in seconds and its default is <pre>0.01</pre>. If that's to fast for you, please consider the option <pre>-t</pre>.</p>
<p><pre>~/.scripts/blurme -t 0.5</pre></p>
<h4>Help</h4>
<p>If you forgot all these parameters just typ:</p>
<p><pre>~/.scripts/blurme -h</pre></p>
