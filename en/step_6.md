## Changing the track

Now that you know how to use the joystick, set it to change which track is playing.

--- task ---
When the program starts, you will need to `stop all sounds`{:class="block3sound"}:

```blocks3
when flag clicked
set [track v] to (1)
display text (join [track] (track)) ::extension
+stop all sounds
set volume to (100) %
start sound (track)
forever
set pixel x (pick random (0) to (7)) y (pick random (0) to (7)) to (pick random (-100000) to (100000)) ::extension
```

--- /task ---

--- task ---

Use the `when joystick pushed`{:class="block3extension"} blocks to change the value stored in your `track`{:class="block3variables"} variable:
```blocks3
when joystick pushed right ::hat extension
stop all sounds
change [track v] by (1)

when joystick pushed left ::hat extension
stop all sounds
change [track v] by (-1)
```

--- /task ---

--- task ---

Add `display text`{:class="block3extensions"} and `start sound`{:class="block3sound"} blocks for both arrow keys.

```blocks3
when joystick pushed right ::hat extension
stop all sounds
change [track v] by (1)
+display text (join [track] (track)) ::extension
+start sound (track)

when joystick pushed left ::hat extension
stop all sounds
change [track v] by (-1)
+display text (join [track] (track)) ::extension
+start sound (track)
```

--- /task ---

--- task ---

Test your code: Click on the green flag and then have a go at changing your tracks using the Sense HAT joystick.

--- /task ---

That's it — your MP3 player is complete! 
