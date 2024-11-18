## Changing the track

Now that you know how to use the joystick, it's time to try to use it to change which track is playing.

--- task ---
1. 

2. Use the `when joystick pushed left`{:class="block3extensions"} and the `when joystick pushed right`{:class="block3extensions"} blocks to `stop all sounds`{:class="block3sound"} and to increase or decrease the value of your `track`{:class="block3variables"} variable.
3. You can also use a `scroll message`{:class="block3extensions"} block to show again which track is being played.
--- /task ---

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

Use the `when arrow is pressed`{:class="block3events"} blocks to change the value stored in your `track`{:class="block3variables"} variable:
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
