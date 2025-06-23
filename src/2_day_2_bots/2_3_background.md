# Task 2.3: Add Background Image
1. Save the image path as a variable: e.g.`background_image = "images/background/wooden_floor.jpeg"`
2. Then load it using `background = pygame.image.load(background_image)`
3. Make sure the background fits the window use `background = pygame.transform.scale(background, (size_x, size_y))`
4. Draw the background onto the screen use `screen.blit(background, (0,0))`

<div style="font-size: 20px; background-color: #96a1de; color: black; padding: 15px; border-radius:10px; text-align: center;">
<p><b>💡 Note </b><p>
<p>Make sure you add your background image <b>before</b> the game loop!</p>
<p>Try adding your own image! JPEGs are preferable since they don't get as blurry when you zoom in on them.</p>
</div>

<br>
<div style="font-size: 20px; background-color: #d9d0f3; color: black; padding: 15px; border-radius:10px;">
    <p style="text-align: center;"><b>🚩 Checkpoint</b><p>
    <ul>  
        <li>A <code>background_image</code> variable (path to the image)</li>
        <li>A <code>background</code> variable (the scaled loaded image)</li>
        <li>A <code>screen.blit(variable, coordinate)</code> line outside your <code>while running:</code> loop</li>
        <li>A background showing up instead of a black screen!</li>
    </ul>
</div>