## Changing the volume

You can now add some extra controls to your MP£ player. First of all you can set up your scripts so that the SenseHAT joystick can control the volume.

The SenseHAT joystic is treated by the computer the same way the cursor keys are on your keyboard. Pushing the joystick up is the same as pushing the up arrow on your keyboard.

--- task ---
Change your intitial script so that the volume starts at `100%`
```blocks
when flag clicked
set [track v] to [1]
scroll message (join [track] (track)) at rotation [0 v] in colour [white v] background [off v] ::extension
set volume to (100) %
play sound (track)
forever
set pixel (pick random (0) to (7)),( pick random (0) to (7)) to R (pick random (0) to (255))G(pick random (0) to (255))B(pick random (0) to (255))::extension
```
--- /task ---

--- task ---
Add in two new scripts, using the `when key pressed`{:class="blockcontrol"} blocks to `change volume`{:class="blocksounds"}.

```blocks
when [up arrow v] key pressed
change volume by (10)

when [down arrow v] key pressed
change volume by (-10)
```
--- /task ---

Test your scripts again by clicking the green flag and then use the SenseHAT joystick to change the volume of your music.
