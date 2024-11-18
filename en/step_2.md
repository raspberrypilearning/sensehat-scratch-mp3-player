## Making it sparkle

Get the Sense HAT to show a random sparkly display to accompany your favorite music.

--- task ---
Open Scratch 3 from the application menu.
[[[rpi-scratch-opening]]]
--- /task ---

--- task ---
Choose a sprite for your MP3 player — in this example, the sprite is a speaker.
![A media player interface displaying a simple illustration of a turquoise speaker with two circular gray and black speakers on its front. At the top, there is a green flag icon and a red stop button for controlling playback.](images/speaker.png)
[[[generic-scratch3-sprite-from-library]]]
--- /task ---

You can delete any scripts or sounds that are already on your sprite.

--- task ---
Add the **Pi SenseHAT** extension in Scratch.
[[[rpi-scratch3-add-sensehat-extension]]]
--- /task ---

Now you're all set up, you can begin to make your MP3 player by creating a disco effect on the display.

--- task ---
Begin by adding a `when flag clicked`{:class="block3events"} block, and then add a `forever`{:class="block3control"} block below it.
```blocks3
when flag clicked
forever
```
--- /task ---

--- task ---
Find the `set pixel`{:class="block3extensions"} block in the Sense HAT extension.
Put numbers into the `x`{:class="block3extensions"} and`y`{:class="block3extensions"} fields, and change the colour in the `to`{:class="block3extensions"} field.
--- /task ---

--- task ---
Test your code. 

Click on the block, and you should see the colour of the pixel on the Sense HAT change.
--- /task ---

--- task ---
Change the pixel position and colour to be random.

```blocks3
set pixel x (pick random (0) to (7)) y (pick random (0) to (7)) to (pick random (-100000) to (100000)) ::extension
```
--- /task ---

--- task ---
Test your code. 

Click on the block again a few times, and you should see random pixels being set to random colours.
--- /task ---

--- task ---
Now place the `set pixel`{:class="block3extensions"} block into your `forever`{:class="block3control"} loop.
--- /task ---

--- task ---
```blocks3
when flag clicked
forever
+set pixel x (pick random (0) to (7)) y (pick random (0) to (7)) to (pick random (-100000) to (100000)) ::extension
end
```
--- /task ---

--- task ---
Test your code. 

Click on the green flag to try running your program. You should see the LEDs on the Sense HAT begin to randomly sparkle.
--- /task ---

