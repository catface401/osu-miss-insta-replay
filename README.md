# osu-miss-insta-replay
### ever miss a note and want to see exactly how? this tool listens for your combobreak sound effect and saves a short video showing your cursor movements and tapping locations so you can get up close and personal to all your shortcomings as a player. 
with this tool you wont improve any faster but you'll sure as hell be more upset with yourself.

Note: this shit is not in great condition. if you watch [my preview video]([url](https://youtu.be/nXulLgs8YY8)) you can get it working yourself, but even then there will be bugs and stuff. this is kind of a proof of concept more than anything else; if i could get it working in full screen i would finish it but i'm not sure how to approach that without breaking osu! tos.

## osu break recorder

this tool listens for a unique break sound in osu!, then saves short video clips of the screen around the time of the break. it overlays your cursor and trail to help you see exactly where a mistake happened.

usage:
run the program with python.
configure settings.
press start to begin listening.

when the break sound is detected, a clip will automatically save to the captures folder (created right next to wherever you ran the .py file).

## controls

wav file: the reference sound to detect (your break sound).

buffer secs: how many seconds of video are kept in memory. higher values = longer clips but more ram usage.

post secs: how long after the break sound to keep recording before finalizing a clip.

threshold db: how loud the sound must be (relative to background) to trigger. increase to reduce false positives.

dot radius: size of the cursor dot in pixels.

dot color: color of the cursor dot.

dot life (secs): how long each cursor dot stays visible before fading.

fps: frames per second of the output video.

scale %: downscales the capture resolution for smaller, faster clips.

monitor: choose which display to capture (if you have more than one).

trail color: color of the cursor trail.

trail width: thickness of the cursor trail line.

trail secs: how long the trail follows behind your cursor.

playback speed %: adjusts the playback speed of the saved clip (100 = real time, 50 = half speed).

### tips:

for fastest saving, keep fps and scale lower.

if you get false triggers, raise the threshold db.

use those sine waves i talk about to make it trigger correctly.
