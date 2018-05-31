## Displaying the track number

Next you're going to display the track number that is playing. You can have a go at this on your own to begin with, and use the hints if you get stuck.

--- task ---
Try the following:
1. Create a new variable called `track`{:class="blockdata"}.
   [[[generic-scratch-add-variable]]]
2.  Use the `scroll message`{:class="blockmoreblocks"} block to display the `track`{:class="blockdata"} number on the SenseHAT.
3. Play the track which you set `track`{:class="blockdata"} to.
--- /task ---

--- hints --- --- hint ---
You can set the `track`{:class="blockdata"} number by doing the following:
```blocks
when flag clicked
set [track v] to [1]
play sound [track_01.mp3]
forever
set pixel (pick random (0) to (7)),( pick random (0) to (7)) to R (pick random (0) to (255))G(pick random (0) to (255))B(pick random (0) to (255))::extension
```
--- /hint --- --- hint ---
The `scroll message`{:class="blockmoreblocks"} block can use the `track`{:class="blockdata"} variable with a `join`{:class="blockoperators"} block. You can choose whichever colours you like.
```blocks
when flag clicked
set [track v] to [1]
scroll message (join [track] (track)) at rotation [0 v] in colour [white v] background [off v] ::extension
play sound [track_01.mp3]
forever
set pixel (pick random (0) to (7)),( pick random (0) to (7)) to R (pick random (0) to (255))G(pick random (0) to (255))B(pick random (0) to (255))::extension
```
--- /hint --- --- hint ---
Finish up the script by changing the track that is being played to the `track`{:class="blockdata"} variable.
```blocks
when flag clicked
set [track v] to [1]
scroll message (join [track] (track)) at rotation [0 v] in colour [white v] background [off v] ::extension
play sound (track)
forever
set pixel (pick random (0) to (7)),( pick random (0) to (7)) to R (pick random (0) to (255))G(pick random (0) to (255))B(pick random (0) to (255))::extension
```
--- /hint --- --- /hints ---
