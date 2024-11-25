## Make it sparkle

Get the Sense HAT to show a random sparkly display to accompany your favourite music.

--- task ---
Open Scratch 3 from the application menu.

--- collapse ---
--- 
title: Scratch on Raspberry Pi
---

If you are using a Raspberry Pi computer, Scratch may already be installed. Click on the **Raspberry Pi** icon to open the menu, then click on **Programming**, then select **Scratch 3**.

If you need to install Scratch, follow this process:
+ Click on the Raspberry Pi icon to open the menu
+ Click on **Preferences**
+ Click on **Recommended Software**
+ Select **Scratch 3**
+ Click on **OK**

![Recommended software dialogue with Scratch 3 selected.](images/recommended-software-scratch-3.png)

See [Scratch 3 Desktop for Raspberry Pi](https://www.raspberrypi.org/blog/scratch-3-desktop-for-raspbian-on-raspberry-pi/){:target="_blank"} for more information.

--- /collapse ---

--- /task ---

--- task ---
Choose a sprite for your MP3 player — in this example, the sprite is a speaker.
![A media player interface displaying a simple illustration of a turquoise speaker with two circular gray and black speakers on its front. At the top, there is a green flag icon and a red stop button for controlling playback.](images/speaker.png)
[[[generic-scratch3-sprite-from-library]]]
--- /task ---

Delete any scripts or sounds that are already on your sprite.

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
Put numbers into the `x`{:class="block3extensions"} and`y`{:class="block3extensions"} fields, and change the colour in the `to`{:class="block3extensions"} field:

```blocks3
when flag clicked
forever
+set pixel x (3) y (5) to [#ffffff]:: extension
```
--- /task ---

--- task ---
Test your code. 

Click on the green flag, and you should see the colour of the pixel at (3,5) on the Sense HAT go white.
--- /task ---

--- task ---
Change the pixel position and colour to be random using the `random`{:class="block3operators"} block.

Make sure the numbers in your code match the ones here:

```blocks3
when flag clicked
forever
+set pixel x (pick random (0) to (7)) y (pick random (0) to (7)) to (pick random (-100000) to (100000)) ::extension
```
--- /task ---

--- task ---
Test your code. 

Click on the green flag to try running your program. You should see the LEDs on the Sense HAT begin to randomly sparkle.
--- /task ---

