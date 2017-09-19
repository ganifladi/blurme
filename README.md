# blurme

<p>blurme v1.0 Codename MEH (My Eyes Hurt) is a small script which will blur your feh set background if any window, or rofi is open. Furthermore there are some switches wich can be found, when calling 'blurme -h'. It allows setting a custom directory (-d), adding (-a) a new program, which will start the transition, setting the transition time (-t), and finally one which will draw some output (-v) to the commandline.</p>
<p>Please feel free to fork it, make pull requests and use it in your own projects.</p>
<p>This is my first project i publish. Please be gentle on me :)</p>
<h2>How to start</h2>
<h3>Requirements</h3>
<p>This script makes use of <b>wmctrl</b> to get the current workspace number and to clarify, whether any window is open. It's essential!</p>
<p>Furthermore you'll need <b>feh</b> to set your background image(s).</p>
<p>And last but not least <b>imagemagick</b> is mandatory to blur the images</p>
<h3>Download and ...</h3>
<ol>
    <li>Download the script</li>
    <li>Place it anywhere you like (e.g. ~/.scripts)</li>
    <li>Make it executable (chmod +x ~/.scripts/blurme)</li>
</ol>
<h2>How to run it</h2>
<h3>Manual start</h3>
<p>Run it once in a terminal of your choice with ~/.scripts/blurme</p>
<h3>Autostart</h3>
<h4>i3</h4>
<p>Add the line "exec --no-startup-id ~/.scripts/blurme &" to your i3 config.</p>
