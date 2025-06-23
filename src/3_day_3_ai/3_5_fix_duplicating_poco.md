# Task 3.5: Fix duplicating Poco
Oh no! There's way too many Pocos! Let's fix that.

1. Inside your `while running:` game loop, **at the very start** of the loop (before drawing the player or foods), draw the background again over the whole screen.
<br>
<div style="font-size: 20px; background-color: #ffebdf; color: black; padding: 15px; border-radius:10px;">
    <p style="text-align: center;"><b>💡 Hint</b></p>
    <ul>  
        <li>Use <code>screen.blit(...)</code> to redraw the background in the while loop</li>
    </ul>
</div>

<br>
<div style="font-size: 20px; background-color: #d9d0f3; color: black; padding: 15px; border-radius:10px;">
    <p style="text-align: center;"><b>🚩 Checkpoint</b></p>
    <ul>  
        <li>Now Poco will move smoothly without leaving any clones behind.</li>
    </ul>
</div>
