# Task 3.4: Create the move method

1. Inside your `Player` class, define a new method called `move()`.
<div style="font-size: 20px; background-color: #ffebdf; color: black; padding: 15px; border-radius:10px;">
    <p style="text-align: center;"><b>💡 Hint</b></p>
    <ul>  
        <li>Use the <code>def</code> keyword.</li>
        <li>Remember to give it just one parameter: <code>self</code>.</li>
    </ul>
</div>

2. Use `pygame.key.get_pressed()` to check which keys are currently being held down and save the result into a variable. This function will return a **dictionary** which can be accessed with the variables in the table below.

3. Check if the player is pressing:

| Key | Action | Pygame dictionary key |
|:----|:-------|:--------------|
| `W` key | Move **up** | pygame.K_w |
| `A` key | Move **left** | pygame.K_a |
| `S` key | Move **down** | pygame.K_s |
| `D` key | Move **right** | pygame.K_d |

<br>
<div style="font-size: 20px; background-color: #ffebdf; color: black; padding: 15px; border-radius:10px;">
    <p style="text-align: center;"><b>💡 Hint</b></p>
    <ul>  
        <li>If the <code>W</code> key is pressed, <strong>decrease</strong> the y position.</li>
        <li>If the <code>S</code> key is pressed, <strong>increase</strong> the y position.</li>
        <li>If the <code>A</code> key is pressed, <strong>decrease</strong> the x position.</li>
        <li>If the <code>D</code> key is pressed, <strong>increase</strong> the x position.</li>
        <li>You can access a dictionary like so: <code>dictionary[dictionary_key]</code></li>
    </ul>
</div>

4. Change the player's image depending on the direction they are moving
<div style="font-size: 20px; background-color: #ffebdf; color: black; padding: 15px; border-radius:10px;">
    <p style="text-align: center;"><b>💡 Hint</b></p>
    <ul>  
        <li>When moving <strong>up</strong>, change the image to <code>poco_up.png</code>.</li>
        <li>When moving <strong>down</strong>, change the image to <code>poco_down.png</code>.</li>
        <li>When moving <strong>left</strong>, change the image to <code>poco_left.png</code>.</li>
        <li>When moving <strong>right</strong>, change the image to <code>poco_right.png</code>.</li>
    </ul>
</div>

<br>
<div style="font-size: 20px; background-color: #d9d0f3; color: black; padding: 15px; border-radius:10px;">
    <p style="text-align: center;"><b>🚩 Checkpoint</b></p>
    <ul>  
        <li>A <code>move()</code> method inside your <code>Player</code> class.</li>
        <li>The method checks which keys are pressed.</li>
        <li>The method updates the player’s <code>position_x</code> and <code>position_y</code>.</li>
        <li>The player image changes when moving!</li>
    </ul>
</div>