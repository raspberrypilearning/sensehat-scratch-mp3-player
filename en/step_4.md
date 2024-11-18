## Displaying the track number

Next, display the number of the track that's currently playing. 

--- task ---

Create a new variable called `track`{:class="block3variables"} and set it to `1`{:class="block3variables"}.

[[[generic-scratch3-add-variable]]]

--- /task ---

--- task ---

Add a `set track to`{:class="block3variables"} block to the top of your script:
```blocks3
when flag clicked
+set [track v] to (1)
start sound [track_01 v]
forever
set pixel x (pick random (0) to (7)) y (pick random (0) to (7)) to (pick random (-100000) to (100000)) ::extension
```
--- task ---

Use the `display text`{:class="block3extensions"} block to display the number stored in `track`{:class="block3variables"} on the Sense HAT.You can choose whichever colours you like.
```blocks3
when flag clicked
set [track v] to (1)
+display text (join [track] (track)) ::extension
start sound [track_01 v]
forever
set pixel x (pick random (0) to (7)) y (pick random (0) to (7)) to (pick random (-100000) to (100000)) ::extension
```

--- /task ---

--- task ---

Play the track with the number stored in your `track`{:class="block3variables"} variable.
```blocks3
when flag clicked
set [track v] to (1)
display text (join [track] (track)) ::extension
+start sound (track)
forever
set pixel x (pick random (0) to (7)) y (pick random (0) to (7)) to (pick random (-100000) to (100000)) ::extension
```

--- /task ---