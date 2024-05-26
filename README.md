# SnakeGame
***This Java code defines a class called Board that extends JPanel and implements the ActionListener interface. The class represents the game board where the snake and apples are drawn and the game logic is implemented.

The class has several instance variables:

B_WIDTH and B_HEIGHT: The dimensions of the game board.
DOT_SIZE: The size of each dot representing the snake and apples.
ALL_DOTS: The total number of dots that can fit on the board.
RAND_POS: The maximum value for generating random positions for the apples.
DELAY: The delay between each game tick.
x[] and y[]: Arrays to store the x and y coordinates of each dot representing the snake.
dots: The current number of dots representing the snake.
apple_x and apple_y: The x and y coordinates of the apple.
leftDirection, rightDirection, upDirection, and downDirection: Booleans indicating the direction of the snake's movement.
inGame: A boolean indicating whether the game is still running.
timer: A Timer object that triggers the game logic at a specified interval.
ball, apple, and head: Images representing the snake, apples, and head of the snake, respectively.
The class has several methods:

initBoard(): Initializes the game board by setting up the key listener, setting the background color, setting the preferred size, loading the images, and initializing the game.
loadImages(): Loads the images for the snake, apples, and head.
initGame(): Initializes the game by setting the initial positions of the snake and apples, starting the timer, and setting the initial number of dots.
paintComponent(Graphics g): Overrides the paintComponent method to draw the game board, including the apples, snakes, and game over message if the game is over.
doDrawing(Graphics g): Draws the game board by drawing the apples, snakes, and game over message if the game is over.
gameOver(Graphics g): Draws the game over message on the game board.
checkApple(): Checks if the snake has eaten an apple and updates the number of dots and the position of the apple if it has.



***This Java code defines a class called Snake that extends JFrame, which is a class in the Java Swing library used to create graphical user interfaces (GUIs). The Snake class represents a simple game of Snake, where the player controls a snake body that moves around the screen.

The code begins by importing necessary libraries, including the EventQueue and JFrame classes from the javax.swing package.

The Snake class has a constructor that calls the initUI() method, which initializes the user interface components. The initUI() method adds a Board component to the JFrame, which is a custom component used to display the game board.

The Snake class also has a main() method, which is the entry point of the application. It uses EventQueue.invokeLater() to invoke the Snake class in the Event Dispatch Thread, which is the thread responsible for handling user events and updating the GUI.

The main() method creates a new instance of the Snake class and sets it visible, making the JFrame visible on the screen.

Overall, this code defines a simple Snake game using Java Swing, where the player controls a snake body that moves around the screen.


move(): Moves the snakes based on the current direction.
checkCollision(): Checks for collisions with the walls and the snake's own body.
locateApple(): Generates a random position for the apple within the game board.
actionPerformed(ActionEvent e): The method called by the timer to perform the game logic. It checks if the game is still running, updates the positions of the snakes and apples, checks for collisions, and repaints the game board.
TAdapter: A nested class that extends KeyAdapter to handle keyboard input for changing the direction of the snakes.
Overall, this code implements a simple game of Snake where the player controls a snake to eat apples and avoid hitting the walls or its own body.
