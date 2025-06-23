# Task 3.3: Create the draw method

1.  Create a new method called `draw`.
<div style="font-size: 20px; background-color: #ffebdf; color: black; padding: 15px; border-radius:10px;">
    <p style="text-align: center;"><b>💡 Hint</b></p>
    <ul>  
        <li>Use the <code>def</code> keyword.</li>
        <li>It should be written <strong>inside</strong> your Food class (at the same indentation level as <code>__init__()</code>).</li>
        <li>This method <strong>won’t take any arguments</strong> (only <code>self</code>).</li>
        <li>This method will <strong>draw the food</strong> onto the screen.</li>
        <li>In general, a method looks like:</li>
        <pre><code>
class Car:
    # These are our properties
    def __init__(self, colour, speed):
        colour = colour
        speed = speed
    ‎ 
    # These are our methods
    def drive(self):
        # Do something here
</code></pre>
    </ul>
</div>

2. Draw the Sprite onto the Screen
<div style="font-size: 20px; background-color: #ffebdf; color: black; padding: 15px; border-radius:10px;">
    <p style="text-align: center;"><b>💡 Hint</b></p>
    <ul>  
        <li>Use <code>screen.blit(...)</code> to draw. Refer to your previous lines of code to see how to use this function!</li>
        <li>The first thing you want to draw is the <strong>sprite</strong>.</li>
        <li>The position to draw at is <code>(position_x, position_y)</code>.</li>
    </ul>
</div>

<br>
<div style="font-size: 20px; background-color: #d9d0f3; color: black; padding: 15px; border-radius:10px;">
    <p style="text-align: center;"><b>🚩 Checkpoint</b></p>
    <ul>  
        <li>A <code>draw()</code> method inside your Player class which knows how to:</li>
        <ul>
            <li>Draw the sprite.</li>
            <li>Place it at the correct position.</li>
        </ul>
    </ul>
</div>