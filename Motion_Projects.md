# PictoBlox Python Motion Projects

A collection of fun programming challenges to practice Python with PictoBlox!

---

## 🎮 Project 1: Ball Movement

![Ball Movement Demo](https://ai.thestempedia.com/wp-content/uploads/2022/08/Ball-Movement-Control.gif)

### What You'll Build
Create a ball that you can control using the arrow keys on your keyboard!

### Your Task
Make a ball sprite that:
- Moves UP when you press the up arrow
- Moves DOWN when you press the down arrow
- Moves LEFT when you press the left arrow
- Moves RIGHT when you press the right arrow

### Skills You'll Learn
- Detecting keyboard input
- Changing sprite position
- Using while loops
- Working with if statements

### Libraries You'll Need
- Motion
- Sensing

### Challenge for You
Can you make the ball move faster or slower? Try changing the movement speed!

---

## 🪲 Project 2: Beetle Movement

![Beetle Movement Demo](https://ai.thestempedia.com/wp-content/uploads/2022/08/Beetle-Movement.gif)

### What You'll Build
Control a beetle sprite that moves and rotates like a real bug!

### Your Task
Make a beetle sprite that:
- Moves FORWARD when you press the up arrow
- Moves BACKWARD when you press the down arrow
- Turns LEFT when you press the left arrow
- Turns RIGHT when you press the right arrow
- Starts at the center of the screen (0, 0)
- Faces to the right when the program starts

### Skills You'll Learn
- Using move() vs changex()/changey()
- Rotating sprites with left() and right()
- Setting starting position
- Setting starting direction

### Libraries You'll Need
- Motion
- Sensing

### Challenge for You
Can you make the beetle turn faster? What happens if you change the rotation speed?

---

## ⚽ Project 3: Bouncing Ball with Gravity

![Bouncing Ball with Gravity Demo](https://ai.thestempedia.com/wp-content/uploads/2022/08/Bouncing-Ball-with-Gravity.gif)

### What You'll Build
Create a realistic bouncing ball that falls down and bounces off the walls!

### Your Task
Make a ball that:
- Starts at a random position on the screen
- Falls down because of "gravity"
- Bounces off all four walls (top, bottom, left, right)
- Slows down a little bit each time (like real friction)
- Moves in a random direction when it starts

### Skills You'll Learn
- Working with variables (gravity, speed, position)
- Using the random module
- Understanding physics concepts (gravity, friction)
- Checking boundaries (when sprite hits edges)
- Advanced math with motion

### Libraries You'll Need
- Motion
- Python's time and random modules

### Challenge for You
Can you make the ball bounce higher? Try changing the gravity value! What happens if you make gravity positive instead of negative?

---

## 🐭 Project 4: Follow the Mouse

![Follow the Mouse Demo](https://ai.thestempedia.com/wp-content/uploads/2022/08/Follow-Mouse.gif)

### What You'll Build
Make a sprite that follows your mouse cursor around the screen!

### Your Task
Make Tobi sprite:
- Always point toward the mouse cursor
- Move towards the mouse continuously
- Follow the mouse smoothly

### Skills You'll Learn
- Using pointto() function
- Creating smooth following motion
- Working with the mouse pointer
- Very simple but cool movement!

### Libraries You'll Need
- Motion

### Challenge for You
Can you make Tobi follow the mouse faster or slower? What happens if you change the move speed from 3 to 10?

---

## 🎯 Project 5: Mouse Tracker

![Mouse Tracker Demo](https://ai.thestempedia.com/wp-content/uploads/2022/08/Mouse-Tracker.gif)

### What You'll Build
Make Tobi jump to wherever you click when you press the spacebar!

### Your Task
Make Tobi sprite:
- Wait for you to press the spacebar
- Jump to the mouse position when spacebar is pressed
- Keep checking for the spacebar continuously

### Skills You'll Learn
- Detecting spacebar presses
- Getting mouse X and Y positions
- Using setx() and sety() functions
- Combining keyboard and mouse sensing

### Libraries You'll Need
- Motion
- Sensing

### Challenge for You
Can you make it work with a different key? Try using the "enter" key instead of spacebar!

---

## 🖼️ Project 6: Mouse Tracking and Stamping

![Mouse Tracking and Stamping Demo](https://ai.thestempedia.com/wp-content/uploads/2022/08/Stamping-Tobi.gif)

### What You'll Build
Create a drawing program where Tobi leaves stamps wherever you click!

### Your Task
Make Tobi sprite:
- Move to the mouse position when spacebar is pressed
- Leave a stamp (copy of itself) at that position
- Clear all stamps when the program starts
- Keep doing this forever

### Skills You'll Learn
- Using the Pen extension
- Stamping sprite images
- Getting mouse coordinates with mousex() and mousey()
- Clearing the stage
- Creating simple drawing programs

### Libraries You'll Need
- Motion
- Sensing
- Pen

### Challenge for You
Can you make Tobi change size before stamping? Or change colors? Check out the Looks library!

---

## 🧭 Project 7: Sprite Direction

![Sprite Direction Demo](https://ai.thestempedia.com/wp-content/uploads/2022/08/Sprite-Direction.gif)

### What You'll Build
Create an arrow that you can rotate and that shows its current direction!

### Your Task
Make an arrow sprite that:
- Starts at the center (0, 0)
- Is made bigger (size 300)
- Rotates LEFT when left arrow is pressed
- Rotates RIGHT when right arrow is pressed
- Shows its current direction in degrees in a speech bubble

### Skills You'll Learn
- Getting sprite direction
- Displaying information with say()
- Converting numbers to text with str()
- Rotating sprites
- Changing sprite size

### Libraries You'll Need
- Motion
- Looks
- Sensing

### Challenge for You
Can you make the arrow point to different angles? What direction is 0 degrees? What about 90? 180?

---

## 🚶 Project 8: Walking Tobi

![Walking Tobi Demo](https://ai.thestempedia.com/wp-content/uploads/2022/06/Tobi-Walking.gif)

### What You'll Build
Make Tobi walk back and forth across the screen with animated walking!

### Your Task
Make Tobi sprite:
- Walk continuously across the screen
- Bounce off the edges (turn around when hitting a wall)
- Switch between two walking costumes to create animation
- Flip direction when bouncing (use 'left-right' rotation style)
- Add small delays to make the walking look smooth

### Skills You'll Learn
- Using bounceonedge() function
- Switching costumes for animation
- Setting rotation styles
- Using time.sleep() for timing
- Creating smooth animations

### Libraries You'll Need
- Motion
- Looks
- Python's time module

### Challenge for You
Can you make Tobi walk faster or slower? What happens if you remove the time.sleep() lines? Can you add more costumes to make the animation smoother?

---

## 🎯 Tips for Success

**Remember to:**
1. Start simple - get the basic movement working first
2. Test your code frequently - run it after adding each new feature
3. Read the error messages - they help you find mistakes
4. Ask questions if you get stuck
5. Have fun experimenting!

**How to Start Each Project:**
1. Open PictoBlox
2. Switch to Python mode
3. Choose (or create) the sprite mentioned in the project
4. Write your code step by step
5. Click the green flag to test!

---

## 📚 What to Study First

Before starting these projects, make sure you understand:
- How to create a sprite
- How to use `while True:` loops
- How to check if keys are pressed
- Basic x and y coordinates (where sprites can move)

Check the Motion Guide document for help with all the motion functions!

---

**Have fun coding! 🚀**

*Remember: Every programmer makes mistakes - they're how we learn!*
