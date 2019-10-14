## Displaying the track number

Next, you're going to display the number of the track that's currently playing. You can have a go at trying this on your own — use the hints if you get stuck.

--- task ---
Try the following:
1. Create a new variable called `track`{:class="block3data"} and set it to `1`.
   [[[generic-scratch3-add-variable]]]
1. Use the `display text`{:class="block3extensions"} block to display the number stored in `track`{:class="block3data"} on the Sense HAT.
1. Play the track with the number stored in your `track`{:class="block3data"} variable.
--- /task ---

--- hints --- --- hint ---
You can store a number in `track`{:class="block3data"} by doing the following:
```blocks3
when flag clicked
set [track v] to (1)
start sound [track_01 v]
forever
set pixel x (pick random (0) to (7)) y (pick random (0) to (7)) to (pick random (-100000) to (100000)) ::extension
```
--- /hint --- --- hint ---
The `display text`{:class="block3extensions"} block can use the `track`{:class="block3data"} variable with a `join`{:class="block3operators"} block. You can choose whichever colours you like.
```blocks3
when flag clicked
set [track v] to (1)
display text (join [track] (track)) ::extension
start sound [track_01 v]
forever
set pixel x (pick random (0) to (7)) y (pick random (0) to (7)) to (pick random (-100000) to (100000)) ::extension
```
--- /hint --- --- hint ---
Finish the script by changing the track that is being played to the `track`{:class="block3data"} variable.
```blocks3
when flag clicked
set [track v] to (1)
display text (join [track] (track)) ::extension
start sound (track)
forever
set pixel x (pick random (0) to (7)) y (pick random (0) to (7)) to (pick random (-100000) to (100000)) ::extension
```
--- /hint --- --- /hints ---
