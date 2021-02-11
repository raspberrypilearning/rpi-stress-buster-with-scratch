## Highs and Lows

In this step, you will learn about the differences between input pins being pulled **High** or **Low**

At the moment, your program looks like this:

```blocks3
when flag clicked
set gpio [17 v] to input [pulled high v] ::extension

when gpio [17 v] is [low v] ::hat extension
move (10) steps
```

You can see that when the **green flag** is clicked, that pin GP17 is set to an **input** and **pulled high**. What does this mean?

--- task ---

Change the dropdowns on the script, to set the pin to an **input** that is **pulled low**. Also change the event block so that is looking for pin GP17 being **High**

```blocks3
when flag clicked
set gpio [17 v] to input [pulled low v] ::extension

when gpio [17 v] is [high v] ::hat extension
move (10) steps
```

Click the green flag and try touching the leads together again. Does the sprite move?

--- /task ---

In the previous project, you learned that an output pin can be set **High** or **Low**. It's either at **3V3** volts or **0V**. What does this mean for input pins though?

Imagine a balloon floating about in the middle of a drafty room. The balloon keeps moving up and down, but how can you tell if it's **High** in the room or **Low** in the room. 

If you tied the balloon to the floor, then you would know that it is as **Low** as it can possible be. If you tied it to the ceiling, then you know that the balloon is as **High** as it can possible be.

Now if cut the tie and the balloon moves, you can easily tell if it moves higher or lower than it's start position.

ANIMATED GIF HERE OF BALLOON

This is what happens when you pull an input pin **Low** or **High**. You are either tieing the pin to be as low as it can be, which is **0V** or tieing it to be as high as it can be, which is **3V3**. Any change in the pin is now easy to detect. It should be either at **0V** or **3V3**, and if it moves from those levels, you know something has changed.

--- task ---

Take the jumper lead that is currently attached to a **ground pin** and move it to a **3V3** pin. A **3V3** pin is always **High**.

![Diagram of a Raspberry Pi with male to female jumper leads attached to pin 17 and a 3V3 pin](images/m-f-3v3.png)

--- /task ---

--- task ---

Now try clicking the green flag and touching the jumper leads together, and see what happens.

--- /task ---

Because your homemade switch is now connected to **3V3**, and the input pin is pulled **Low**, when you touch the leads together, the input pin goes from **Low** at **0V** to **High** at **3V3** volts, and Scratch detects this and so moves your sprite.