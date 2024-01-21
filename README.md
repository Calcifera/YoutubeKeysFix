# YouTube key shortcuts FIX

This is a userscript for web browsers to:
- make YouTube keyboard controls (arrow keys) more intuitive,
- fix annoyances like focusing volume slider and progressbar,
- enable volume control by mousewheel scrolling over the player,
- make Tab-navigation more user-friendly by visualizing focus on player, video list items, comments with frame shadow.

Userscript registry page:  https://greasyfork.org/en/scripts/38643-youtube-key-shortcuts-fix  
[Installation instructions](#installation) below.



### Features

#### Youtube player controls will work consistently when player is focused:
- Left / Right (5sec backwards / forwards), Up / Down (volume up / down), Home (restart video), End (skip to end)
- 0-9 (jump to 0%-90%), C (switch closed captions/subtitles), +/- (change cc font size):  unaffected

#### Player is focused right after pageload, no need to click in player frame:
- Click outside player frame to get standard page controls: Up, Down, Left, Right (scroll)
- Press Esc to focus player, Shift-Esc to cycle search box, video list, like buttons / comments.
- Space pauses video on the whole webpage except textboxes.

#### Global shortcuts, changed:
- Esc (exit fullscreen):  additionally focuses player when not in fullscreen
- Space (play/pause):  works on whole page, not only when player is focused

#### Global shortcuts, unaffected:
- F (fullscreen), M (mute)
- K (play/pause)
- J / L (10sec backwards / forwards)
- , (previous frame), . (next frame)
- Shift-, (speed -0.25), Shift-. (speed +0.25)
- Shift-N (next video), Shift-P (previous video)
- / (focus searchfield, only in classic ui)
- ENTER (push the focused button)

#### Fixes the following awkward behaviour of Youtube player controls after clicking them (making the individual control focused):
- after clicking the mute button Space toggles mute instead of pausing
- after clicking the progressbar Up/Down will jump 10 sec in the video instead of changing the volume
- after clicking the volume slider Left/Right will change the volume instead of jumping the video.
- after clicking subtitle button Space will toggle subtitles
- after clicking settings button Space will toggle settings
- after clicking fullscreen button Space will toggle fullscreen

#### YouTube keyboard shortcuts documentation:
- https://shortcutworld.com/Youtube-Player/win/Youtube-Player_Shortcuts
- https://www.hongkiat.com/blog/useful-youtube-keyboard-shortcuts-to-know/
- https://support.google.com/youtube/answer/7631406?hl=en
- 2010 (flash player?) - https://www.makeuseof.com/tag/comprehensive-guide-youtube-player-keyboard-shortcuts/



### Installation

Install an addon to manage userscripts, for example one of the following:
- [Violentmonkey](https://violentmonkey.github.io/)
- [FireMonkey](https://addons.mozilla.org/en-US/firefox/addon/firemonkey/) (FireFox only)
- [Tampermonkey](https://www.tampermonkey.net/)
- [GreaseMonkey](https://addons.mozilla.org/en-US/firefox/addon/greasemonkey/) (FireFox only)

Then install the userscript from the registry:
- https://update.greasyfork.org/scripts/38643/Youtube%20key%20shortcuts%20FIX.user.js

Or install directly from this repository:
- https://github.com/Calciferz/YoutubeKeysFix/raw/main/YoutubeKeysFix.user.js

For the latest in-development version install from the [`dev`](https://github.com/Calciferz/YoutubeKeysFix/tree/dev), branch (not guaranteed to be reliable):
- https://github.com/Calciferz/YoutubeKeysFix/raw/dev/YoutubeKeysFix.user.js

