# Task 3.2: Create an instance of player
If a class is a blueprint, then creating an instance is using that blueprint to make something!

1. Outside of your class definition (in your main code), create a new player object!

<br>
<div style="font-size: 20px; background-color: #ffebdf; color: black; padding: 15px; border-radius:10px;">
    <p style="text-align: center;"><b>💡 Hint</b></p>
    <ul>  
        <li>Generally, you can create a class instance like so:</li>
        <pre><code>
car_instance = Car("Red", 60)
        </code></pre>
        <li>This creates an instance of a car with the colour "Red" and a speed of 60. </li>
        <li>Note: this assumes you have made a class called Car with the properties colour and speed. You can look at 3.1 to see an example of this.</li>
        <li>Your Player class has the properties position_x, position_y, size, image, sprite.</li>
        <li>You should add values inside the bracket, e.g. Player(...) that lines up with those properties.</li>
    </ul>
</div>

2.  After you create the player instance, print out the player’s important properties to check they were created correctly.
<div style="font-size: 20px; background-color: #ffebdf; color: black; padding: 15px; border-radius:10px;">
    <p style="text-align: center;"><b>💡 Hint</b></p>
    <ul>  
        <li>You can access a class property by using a dot, like this: <code>car_instance.colour</code>. This should be"Red".</li>
        <li>Print the player's <code>sprite</code>.</li>
        <li>Print the player's <code>position_x</code>.</li>
        <li>Print the player's <code>position_y</code>.</li>
        <li>Print the player's <code>size</code>.</li>
    </ul>
</div>

<br>
<div style="font-size: 20px; background-color: #d9d0f3; color: black; padding: 15px; border-radius:10px;">
    <p style="text-align: center;"><b>🚩 Checkpoint</b></p>
    <ul>  
        <li>A player object stored in a variable called <code>Player</code>.</li>
        <li>Printouts in the terminal showing the player's properties.</li>
    </ul>
</div>