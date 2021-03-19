--- question ---

---
legend: Question 2 of 3
---

Which of the following event blocks would you use to detect the press of a button on pin 21?

--- choices ---

- ( ) 1:

```blocks3
when button (21 v) is [released v] ::extension
```
--- feedback ---

No. This block is set up to detect if the button is released, not pressed.

--- /feedback ---

- ( ) 2: 
```blocks3
when button (1 v) is [pressed v] ::extension
```

--- feedback ---

No. This block is detecting presses to a button on pin 1, not pin 21.

--- /feedback ---

- ( ) 3: 
```blocks3
when button (21 v) is [pressed v] ::extension
```

--- feedback ---

Yes! This block will detect any presses on a button attached to 21, and then trigger the blocks attached to it.

--- /feedback ---

- ( ) 4: 
```blocks3
when flag clicked
```

--- feedback ---

No. This block will only detect the even of the green flag being clicked. I will not detect any buttons.

--- /feedback ---

--- /choices ---

--- /question ---