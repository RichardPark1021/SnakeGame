# Group Member: Richard, William, Marvin

# SimpleSnakeGame

## Initialization and main method: 
It initialize the screen size and the per unit of pixels.
Initialize the snake location and body parts. It also initialize the apple coordinates. The initial
direction of the snake is right. At the start the game is not running. It also initialize the timer of the game.
The main method create the frame and the panel. Creates a closing option to end the game. Set the title of the game.
Can't resize the screen. The location of the screen will be at the center. It also make the screen visible.

## Class variables:
The class variables are SIZE, UNIT_SiZE, GAME_UNITS, and DELAY.


## SimpleSnakeGame constructor:
The constructor creates the JPanel by setting the size of the panel and setting the background black.
The .addkeylistener allow the to listen the key press. It also runs the game.

## startGame method:
Creates an apple, it runs the game, creates the timer, and starts the timer.

## newApple method:
When the snake eats the apple, the game will create a new apple at a random location.

## paintComponent method:
The paint component will draw the snake and the apple

## draw method:
If the game is running, the game will draw the body(dark green) and head(green) of the snake in a rectangle shape. It also draws
the red apple in a oval shape. When the snake eats the apple, the game will draw a new body for the snake. It 
also creates the game over screen.

## move method: 
The move method moves the body and the head to the next unit of the direction that the head was at. Pressing
the arrow keys on the keyboard allows the snake to change direction.

## checkApple method:
In a if-statement, it checks if the snake eats the apple. If it does eat the apple, then the body part will increase
and the number of apples eaten will also increase. It will also create a new apple.

## checkCollisions method:
In this method it checks if the snake hit the walls or if it touches it's own body. If it does hit anything other 
than the apple, then the game will stop running. The timer will also stop.

## gameOver method:
The gameOver method create the game over screen with a font and color.

## actionPerformed method:
If the game is running, then it checks each method of move(), checkApple(), and checkCollision(). It will also update 
the game by redrawing each object. 

## MyKeyAdapter class:
The keyPressed allow the program to know which direction to go, if we press on a certain key