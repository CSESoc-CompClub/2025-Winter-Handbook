# Task 2.1: Create Game Screen

Before we make our game we need to set up the screen to display it!

1. Create some variables that will hold the width and the height. 800 pixels wide and 600 pixels tall

    E.g. A screen that is 100 pixels wide and 200 pixels could have these variables:

    ```python
        WIDTH = 100
        HEIGHT = 200
    ```

2. Create a window of that size and assign it to screen like so:
```python
pygame.display.set_mode((WIDTH, HEIGHT))
```

<br>
<div style="font-size: 20px; background-color: #96a1de; color: black; padding: 15px; border-radius:10px; text-align: center;">
    <p><b>📝 Note</b><p>
    <p>  
        Running your game will cause your program to crash. You must <b>complete Task 1.2</b> before you can see a screen when you run your pygame.
    </p>
</div>

<br>
<div style="font-size: 20px; background-color: #d9d0f3; color: black; padding: 15px; border-radius:10px;">
    <p style="text-align: center;"><b>🚩 Checkpoint</b><p>
    <ul>  
        <li>Two variables for width and height</li>
        <li>A screen object created using Pygame and your variables</li>
    </ul>