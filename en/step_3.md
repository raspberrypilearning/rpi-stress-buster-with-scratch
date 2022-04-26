## Adding a switch to a game

The stress-relieving [Stress ball](https://projects.raspberrypi.org/en/projects/stress-ball) project is perfect for adding a physical controller to. If you haven't already done so, you can make your own version of the game by following the instructions, or you can [download the finished project](https://rpf.io/p/en/stress-ball-get).

--- task ---

Open the Stress ball Scratch project on your Raspberry Pi, using the Desktop version.

--- collapse ---
---
title: Opening a downloaded Scratch 3 Desktop project
---

Once you have downloaded the zip file from the link above, open your file manager and navigate to the **Downloads** folder.

Find the file you just downloaded. It will end in `.zip`.

Right click on the file and choose 'Extract files'. Extract them to your downloads folder.

In Scratch 3 Desktop, click the `File` menu and choose `Load from your computer`.

Navigate to your downloads folder again and select the file `Stress Ball - challenge.sb3`. 

Click `OK` or press `Enter`.


--- /collapse ---

--- /task ---

--- task ---

Play the game, clicking on the stress ball to squeeze it.

--- /task ---

--- task ---

Add the Raspberry Pi `Simple Electronics`{:class="block3extensions"} extension to your project.

--- /task ---

--- task ---

Just like you did in the last step, add a `when button 21 is pressed`{:class='block3extensions'} block to the code.

```blocks3
when button (21 v) is [pressed v] ::extension hat
```

--- /task ---

The blocks that detect the **Click** and make the **Ball** sprite change, look like this:

```blocks3
when this sprite clicked
set [whirl v] effect to (100)
change size by (-50)
play sound (Squeaky Toy v) until done
clear graphic effects
set size to (200) %
```

--- task ---

Right click on the `set [whirl v] effect to (100)`{:class='block3looks'} block and choose **Duplicate** from the menu.

--- /task ---

--- task ---

Take the newly duplicated blocks and add them underneath the `when button 21 is pressed`{:class='block3extensions'} block, so that your blocks look like this.

```blocks3
when button (21 v) is [pressed v] ::extension hat
set [whirl v] effect to (100)
change size by (-50)
play sound (Squeaky Toy v) until done
clear graphic effects
set size to (200) %
```

--- /task ---

--- task ---

Run your program by clicking the green flag. You should be able to squeeze your **Ball** sprite by touching the jumper wires together.

--- /task ---

--- save ---
