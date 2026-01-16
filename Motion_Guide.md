# PictoBlox Python Motion Library - Simple Guide

## What is Motion?

Motion helps you move sprites (characters) around the screen! Think of it like controlling a character in a video game.

---

## Setting Up Your Sprite

Before using any motion functions, you need to create a sprite object:

```python
sprite = Sprite('Tobi')  # Use the name of your sprite
```

**Note:** Replace `'Tobi'` with the actual name of your sprite in PictoBlox (e.g., `'Beetle'`, `'Cat'`, `'Ball'`).

---

## Moving Your Sprite

### **move(steps)**
Moves your sprite forward by the number of steps you choose.

```python
import time

sprite = Sprite('Tobi')

# Move forward 10 steps
sprite.move(10)
time.sleep(1)

# Move forward 50 steps
sprite.move(50)
```

---

### **right(degrees)** and **left(degrees)**
Turn your sprite right or left, like spinning around!

```python
# Turn right 90 degrees (makes a right turn)
sprite.right(90)

# Turn left 45 degrees (turns a little bit left)
sprite.left(45)
```

---

## Placing Your Sprite Exactly Where You Want

### **gotoxy(x, y)**
Jump to any spot on the screen instantly!
- **x** = left/right position (-240 to 240)
- **y** = up/down position (-180 to 180)
- Center of screen is (0, 0)

```python
# Jump to the top-right corner
sprite.gotoxy(200, 150)

# Jump to the bottom-left corner
sprite.gotoxy(-200, -150)

# Jump back to center
sprite.gotoxy(0, 0)
```

---

### **goto(target)**
Make your sprite jump to another sprite's location, the mouse pointer, or a random position!

```python
# Go to where the mouse pointer is
sprite.goto("_mouse_")

# Go to a random position
sprite.goto("_random_")

# Go to where "Cat" sprite is
sprite.goto("Cat")
```

---

## Changing Position Little by Little

### **changex(value)** and **changey(value)**
Move your sprite a little bit left/right or up/down.

```python
# Move 20 steps to the right
sprite.changex(20)

# Move 30 steps down
sprite.changey(-30)
```

---

### **setx(x)** and **sety(y)**
Put your sprite at an exact x or y position.

```python
# Put sprite at x = 100 (pretty far right)
sprite.setx(100)

# Put sprite at y = -50 (a bit below center)
sprite.sety(-50)
```

---

## Controlling Direction

### **setdirection(angle)**
Point your sprite in any direction:
- 0° = up
- 90° = right
- 180° (or -180°) = down
- -90° = left

```python
# Point up
sprite.setdirection(0)

# Point right
sprite.setdirection(90)

# Point down
sprite.setdirection(180)

# Point left
sprite.setdirection(-90)
```

---

### **pointto(target)**
Make your sprite turn to face another sprite or the mouse pointer!

```python
# Turn to face the "Ball" sprite
sprite.pointto("Ball")

# Turn to face the mouse pointer
sprite.pointto("_mouse_")
```

---

## Special Motion Features

### **bounceonedge()**
Makes your sprite bounce back when it hits the edge of the screen (like a bouncing ball!).

```python
# Move forward and bounce off edges
sprite.move(10)
sprite.bounceonedge()
```

---

### **setrotationstyle(style)**
Choose how your sprite rotates:
- **"all around"** = sprite can spin in any direction (default)
- **"left-right"** = sprite flips when turning left/right
- **"don't rotate"** = sprite never rotates, always faces as if at 90°

```python
# Make sprite flip left and right only
sprite.setrotationstyle("left-right")

# Make sprite spin freely in any direction
sprite.setrotationstyle("all around")

# Make sprite never rotate
sprite.setrotationstyle("don't rotate")
```

---

## Getting Information About Your Sprite

### **x()**, **y()**, **direction()**
Find out where your sprite is and which way it's facing!

```python
# Get current x position
current_x = sprite.x()
print("I am at x:", current_x)

# Get current y position
current_y = sprite.y()
print("I am at y:", current_y)

# Get current direction
current_direction = sprite.direction()
print("I am facing:", current_direction, "degrees")
```

---

## 🎮 Fun Example Program: Make a Square!

```python
import time

sprite = Sprite('Tobi')

# Draw a square by moving and turning!
for i in range(4):  # Do this 4 times
    sprite.move(100)      # Move forward 100 steps
    time.sleep(0.5)       # Wait a moment
    sprite.right(90)      # Turn right 90 degrees
    time.sleep(0.5)       # Wait a moment

print("I made a square!")
```

---

## 🌟 Fun Example Program: Sprite Dance!

```python
import time

sprite = Sprite('Tobi')

# Dance around the screen!
sprite.gotoxy(0, 0)  # Start in the middle

# Spin around
for i in range(8):
    sprite.right(45)
    sprite.move(50)
    time.sleep(0.3)

# Jump to random spots
sprite.gotoxy(100, 100)
time.sleep(0.5)
sprite.gotoxy(-100, -100)
time.sleep(0.5)
sprite.gotoxy(100, -100)
time.sleep(0.5)
sprite.gotoxy(-100, 100)

print("Dance complete!")
```

---

## Quick Tips! 🎯

1. **Positive numbers** = right and up
2. **Negative numbers** = left and down
3. **Always use `time.sleep()`** to see your sprite move (or it goes too fast!)
4. **Start simple** - try moving forward, then add turns!

Have fun making your sprites move! 🚀

---

## Quick Reference Table

| Function | What it does | Example |
|----------|-------------|---------|
| `move(steps)` | Move forward | `sprite.move(50)` |
| `right(degrees)` | Turn right | `sprite.right(90)` |
| `left(degrees)` | Turn left | `sprite.left(45)` |
| `gotoxy(x, y)` | Jump to position | `sprite.gotoxy(100, 50)` |
| `goto(target)` | Jump to target | `sprite.goto("_mouse_")` |
| `changex(value)` | Move left/right | `sprite.changex(20)` |
| `changey(value)` | Move up/down | `sprite.changey(-30)` |
| `setx(x)` | Set x position | `sprite.setx(100)` |
| `sety(y)` | Set y position | `sprite.sety(-50)` |
| `setdirection(angle)` | Point in direction | `sprite.setdirection(90)` |
| `pointto(target)` | Face a target | `sprite.pointto("Ball")` |
| `bounceonedge()` | Bounce off screen edges | `sprite.bounceonedge()` |
| `setrotationstyle(style)` | Change rotation style | `sprite.setrotationstyle("left-right")` |
| `x()` | Get x position | `current_x = sprite.x()` |
| `y()` | Get y position | `current_y = sprite.y()` |
| `direction()` | Get direction | `angle = sprite.direction()` |

---

**Made with ❤️ for Young Python Learners**
