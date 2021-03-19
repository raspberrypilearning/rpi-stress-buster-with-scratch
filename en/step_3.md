## Adding a switch to a game

The [Stress ball](https://projects.raspberrypi.org/en/projects/flappy-parrot) project is a stress relieving program that you can add a physical controller to. You can either use the instructions to create the game yourself, or you can download the finished project at [rpf.io/en/p/stress-ball-get](https://rpf.io/en/p/stress-ball-get).

--- task ---

Open the Stress ball Scratch project on your Raspberry Pi, using the Desktop version.

--- /task ---

--- task ---

Play the game, using the by clicking on the stress ball to squeeze it.

--- /task ---

--- task ---

Add the **Raspberry Pi Simple Electronics** extension to your project.

--- /task ---

--- task ---

Just like you did in the last step, add a `when button 21 is pressed`{:class='block3extensions'} block to the code.

```blocks3
when button (21 v) is [pressed v] ::extension hat
```

--- /task ---

The blocks that detect the **Click** and make `Ball` change, look like this:

```blocks3
when this sprite clicked
set [whirl v] effect to (100)
change size by (-50)
play sound (Squeaky Toy v) until done
clear graphic effects
set size to (200) %
```

--- task ---

Right click on the `set [whirl v] effect to (100)`{:class='block3looks'} block and choose `Duplicate` from the menu.

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

Run your program by clicking the green flag. You should be able to squeeze your `Ball` up, by touching the jumper leads together.

--- /task ---

--- save ---