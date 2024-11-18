## Displaying the track number

Next, display the number of the track that's currently playing. 

--- task ---

Create a new variable called `track`{:class="block3variables"} and set it to `1`{:class="block3variables"} at the top of your script:

[[[generic-scratch3-add-variable]]]

```blocks3
when flag clicked
+set [track v] to (1)
start sound [Coding Bliss v]
forever
set pixel x (pick random (0) to (7)) y (pick random (0) to (7)) to (pick random (-100000) to (100000)) ::extension
```


--- /task ---

--- task ---
Use the `display text`{:class="block3extensions"} block to display the number stored in `track`{:class="block3variables"} on the Sense HAT:
```blocks3
when flag clicked
set [track v] to (1)
+display text (join [track] (track)) ::extension
start sound [Coding Bliss v]
forever
set pixel x (pick random (0) to (7)) y (pick random (0) to (7)) to (pick random (-100000) to (100000)) ::extension
```
--- /task ---

--- task ---
Play the track with the number stored in your `track`{:class="block3variables"} variable:
```blocks3
when flag clicked
set [track v] to (1)
display text (join [track] (track)) ::extension
+start sound (track)
forever
set pixel x (pick random (0) to (7)) y (pick random (0) to (7)) to (pick random (-100000) to (100000)) ::extension
```
--- /task ---