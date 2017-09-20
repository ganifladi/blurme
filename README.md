# blurme

<p>blurme v1.0 Codename MEH (My Eyes Hurt) is a small script which will blur your feh set background if any window, or rofi is open. Furthermore there are some options, which allow you to change the default behaviour a bit. Read more about the options down below.</p>
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
<p>Add the line "sh ~/.scripts/blurme &" to ~/.xinitrc</p>
<h4>openbox</h4>
<p>Add the line "sh ~/.scripts/blurme &" to ~/.config/openbox/autostart</p>
<h3>Options</h3>
<p>There are several optional arguments provided that may be used. These include:</p>
<ul>
    <li><b>-a</b>: Add another program (process name), which will start the blur effect</li>
    <li><b>-c</b>: set custom directory for transition images (default: ~/.cache/blurme)</li>
    <li><b>-d</b>: Set custom directory (defaul ~/.local/share/blurme)</li>
    <li><b>-t</b>: Set custom transition time in sec (default: 0.01)</li>
    <li><b>-v</b>: Show additional output (verbose)</li>
    <li><b>-h</b>: Show all these parameters</li>
</ul>
