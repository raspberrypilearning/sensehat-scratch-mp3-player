## Making it sparkle

Let's being by using the SenseHAT to produce a random sparkly display, to accompnay your favorite music.

--- task ---
Open Scratch 2 from the application menu.
[[[rpi-scratch-opening]]]
--- /task ---

--- task ---
Choose a sprite for your MP3 player - here we're going to use a speaker.
![speaker](images/speaker.png)
[[[generic-scratch-sprite-from-library]]]
--- /task ---

You can delete any scripts or sounds that are already on your sprite.

--- task ---
Add the SenseHAT extension in Scratch.
[[[rpi-scratch-add-pi-sense-hat]]]
--- /task ---

Now you're all setup, you can begin creating your MP3 player by creating a disco effect on the display, to acccompany the songs.

--- task ---
Begin by adding a `when flag clicked`{:class="blockevents"}, and then add a `forever`{:class="blockcontrol"} beneath it.
```blocks
when flag clicked
forever
```
--- /task ---

--- task ---
Within the `More Blocks`{:class="blockmoreblocks"} menu you can find the `set pixel`{:class="blockmoreblocks"} block. By using the `pick random`{:class="blockoperators"} block you can set random pixel positions and random colours within the loop, to make the SenseHAT sparkle

```blocks
when flag clicked
forever
set pixel (pick random (0) to (7)),( pick random (0) to (7)) to R (pick random (0) to (255))G(pick random (0) to (255))B(pick random (0) to (255))::extension
```
--- /task ---

--- task ---
Have a go at running your program by clicking on the Green flag. You should see the LEDs on the SenseHAT ranndomly begin to sparkle.
--- /task ---

