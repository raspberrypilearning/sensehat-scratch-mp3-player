## Changing the volume

You can now add some extra controls to your MP3 player. First of all, set up your script so that the Sense HAT joystick can control the volume.

The Raspberry Pi treats the Sense HAT joystick in the same way as the arrow keys on your keyboard. This means that, for example, pushing the joystick up is the same as pushing the up arrow on your keyboard.

--- task ---
Change the script you already have so that the volume starts at `100%`{:class="block3sound"}.
```blocks3
when flag clicked
set [track v] to (1)
display text (join [track] (track)) ::extension
set volume to (100) %
start sound (track)
forever
set pixel x (pick random (0) to (7)) y (pick random (0) to (7)) to (pick random (-100000) to (100000)) ::extension
```
--- /task ---

--- task ---
Add in two new scripts that use `when joystick pushed`{:class="block3extensions"} blocks to `change volume`{:class="block3sound"}.

```blocks3
when joystick pushed [up v] ::extension
change volume by (10)

when joystick pushed [down v] ::extension
change volume by (-10)
```
--- /task ---

Test your scripts again: click the green flag, and then use the Sense HAT joystick to change the volume of your music.
