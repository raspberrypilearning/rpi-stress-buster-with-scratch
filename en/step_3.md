## Keys vs switches

At the moment you have two ways of moving the sprite. You can press the **space key** or you can touch the jumper leads together.

--- task ---

Hold down the **space key** on your keyboard for a few seconds and see what happens.

--- /task ---

--- task ---

Now drag the sprite back to the centre of the screen and hold the jumper leads together for a few seconds and see what happens.

--- /task ---

Computers don't just read a pressed key as **on**. Instead they read it as lots of **ons** then **offs**. This is why when you are typing and you hold down a key, a long line of characters is produced. It also means that in your project, the sprite keeps moving.

Your switch sends just a single **on** though, so your sprite only moves once. You can make your switch behave like a keyboard key, using some code.

--- task ---

Remove all you code blocks, by dragging them back to the **blocks palate** 

--- /task ---

--- task ---

Now you can use a `forever`{:class='block3control'} loop, with an `if...then`{:class='block3control'} block inside to constantly check if the switch is pressed.

```blocks3
when flag clicked
forever
if <button (17 v) is [pressed v]? ::extension> then
move (10) steps
```

--- /task ---

--- task ---

Run your program by clicking the green flag, then touch your jumper leads together, and your sprite should keep moving 10 steps.

--- /task ---

--- save ---