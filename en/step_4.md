## Adding a switch to a game

The [Flappy Parrot](https://projects.raspberrypi.org/en/projects/flappy-parrot) project is a game that you can add a physical controller to. You can either use the instructions to create the game yourself, or you can remix this finished [Scratch project](https://scratch.mit.edu/projects/258349724/).

--- task ---

Open the Flappy Parrot Scratch project on your Raspberry Pi, or if you are using the online project, save it to your Raspberry Pi, and open it in your offline version of Scratch.

Play the game, using the **Space key** to control the `Flappy` sprite.

--- /task ---

--- task ---

Add the **Raspberry Pi Simple Electronics** extension to your project.

--- /task ---

--- task ---

Click on the `Flappy` sprite to see the code that is attached to it.

--- /task ---

--- task ---

Just like you did in the last step, add a `forever`{:class='block3control'} loop to always detect the button press.

```blocks3
when flag clicked
forever
if <button (17 v) is [pressed v]? ::extension> then
```

--- /task ---

The blocks that detect the **Space key** being pressed and make `Flappy` fly, look like this:

```blocks3
when [space v] key pressed
switch costume to (wings down v)
repeat (5) 
  change y by (6)
end
switch costume to (wings up v)
repeat (5) 
  change y by (6)
end
```

--- task ---

Right click on the `switch costume to wings-down`{:class='block3looks} block and choose `Duplicate` from the menu.

--- /task ---

--- task ---

Take the newly duplicated blocks and add them into you `if...then`{:class='block3control'} block, so that your blocks look like this.

```blocks3
when flag clicked
forever
if <button (17 v) is [pressed v]? ::extension> then
when [space v] key pressed
switch costume to (wings down v)
repeat (5) 
  change y by (6)
end
switch costume to (wings up v)
repeat (5) 
  change y by (6)
end
```

--- /task ---

--- task ---

Run your program by clicking the green flag. You should be able to move `Flappy` up, by touching the jumper leads together and let `Flappy` fall by taking them apart.

--- /task ---