## Changing the track

Now that you know how to use the joystick, it's time to try to use it to change which track is playing.

--- task ---
1. When the program starts, you will need to `stop all sounds`{:class="block3sound"}.

2. Use the `when joystick pushed left`{:class="block3extensions"} and the `when joystick pushed right`{:class="block3extensions"} blocks to `stop all sounds`{:class="block3sound"} and to increase or decrease the value of your `track`{:class="block3variables"} variable.
3. You can also use a `scroll message`{:class="block3extensions"} block to show again which track is being played.
--- /task ---

--- hints --- --- hint ---
Adding a single block will complete your main script:
```blocks3
when flag clicked
set [track v] to (1)
display text (join [track] (track)) ::extension
stop all sounds
set volume to (100) %
start sound (track)
forever
set pixel x (pick random (0) to (7)) y (pick random (0) to (7)) to (pick random (-100000) to (100000)) ::extension
```
--- /hint --- --- hint ---
You can use the `when arrow is pressed`{:class="block3events"} blocks to change the value stored in your `track`{:class="block3variables"} variable like this:
```blocks3
when joystick pushed right ::hat extension
stop all sounds
change [track v] by (1)

when joystick pushed left ::hat extension
stop all sounds
change [track v] by (-1)
```
--- /hint --- --- hint ---
Then you just need to `scroll message`{:class="block3extensions"} and `play sound`{:class="block3sound"} for both arrow keys.

```blocks3
when joystick pushed right ::hat extension
stop all sounds
change [track v] by (1)
display text (join [track] (track)) ::extension
start sound (track)

when joystick pushed left ::hat extension
stop all sounds
change [track v] by (-1)
display text (join [track] (track)) ::extension
start sound (track)
```
--- /hint --- --- /hints ---

That's it — your MP3 player is complete! Click on the green flag and then have a go at changing your tracks using the Sense HAT joystick.
