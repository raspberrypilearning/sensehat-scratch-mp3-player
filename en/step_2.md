## Making it sparkle

Let's being by getting the Sense HAT to show a random sparkly display to accompany your favorite music.

--- task ---
Open Scratch 2 from the application menu.
[[[rpi-scratch-opening]]]
--- /task ---

--- task ---
Choose a sprite for your MP3 player — here we're going to use a speaker.
![speaker](images/speaker.png)
[[[generic-scratch3-sprite-from-library]]]
--- /task ---

You can delete any scripts or sounds that are already on your sprite.

--- task ---
Add the **Pi SenseHAT** extension in Scratch.
[[[rpi-scratch3-add-sensehat-extension]]]
--- /task ---

Now you're all set up, you can begin to make your MP3 player by creating a disco effect on the display.

--- task ---
Begin by adding a `when flag clicked`{:class="blockevents"} block, and then add a `forever`{:class="blockcontrol"} block below it.
```blocks3
when flag clicked
forever
```
--- /task ---

--- task ---
Find the `set pixel`{:class="block3extension"} block in the Sense Hat extension.
Try adding numbers into the `x`{:class="block3extension"}, `y`{:class="block3extension"} and changing the colour in the `to`{:class="block3extension"} field.

Then click the block and you should see the colour of the pixel on the Sense HAT change.
--- /task ---

--- task ---
Now you can change the pixel position and colour to be random.

```blocks3
set pixel x (pick random (0) to (7)) y (pick random (0) to (7)) to (pick random (-100000) to (100000)) ::extension
```

Click on the block again and you should see random pixels being set to random colours
--- /task ---

--- task ---
Now place the `set pixel`{:class="block3extension"} into your `forever`{:class="block3control"} loop.
--- /task ---

--- task ---
```blocks3
when flag clicked
forever
set pixel x (pick random (0) to (7)) y (pick random (0) to (7)) to (pick random (-100000) to (100000)) ::extension
```
--- /task ---

--- task ---
Have a go at running your program by clicking on the green flag. You should see the LEDs on the Sense HAT begin to randomly sparkle.
--- /task ---

