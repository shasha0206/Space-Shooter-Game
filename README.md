# Space-Shooter-Game

Code Overview
The code consists of several key components and functions:

Initialization
The game initializes using pygame.init(), sets the caption to 'Space Shooter', and sets up the game window with a resolution of 1000x750 pixels.

Game Variables
Key game variables include game_over, game_end, clock, screen_width, and screen_height.

Ship Details
The spaceship is initialized with a width and height of 80 pixels, positioned at the center-bottom of the screen.

Laser Details
Lasers are defined with a width of 20 pixels and a height of 80 pixels.

Meteor Details
Meteors have a width and height of 40 pixels and are stored in a list called meteors_list.

Functions
create_meteros(num): Generates a specified number of meteors at random positions.
create_stars(num): Generates a specified number of stars at random positions.
creat_heart(): Initializes the player's hearts (lives).
create_sl(num): Creates special lasers.
create_laser(num): Creates regular lasers.
movement(): Handles the spaceship's movement based on key presses.
collision(ship_rect): Detects and handles collisions between the spaceship, meteors, lasers, and special lasers.
Graphics
The game loads and scales various images for the background, stars, ship, meteors, lasers, hearts, explosions, and game over screen.

Heart Details
The player's hearts are created and displayed using the creat_heart() function.

Special Laser
Special lasers are created and managed similarly to regular lasers but have a different appearance and behavior.

Collisions
The collision() function detects and handles collisions between the spaceship, meteors, lasers, and special lasers. It updates the game state accordingly.

High Score
The game reads and updates the high score from a file (highscore.txt). The high score is updated if the current game timer exceeds the previous high score.

Timers
The game uses custom timers for meteor creation (meteor_timer) and manages the timing for laser and special laser shots.

Game Timer
The game calculates and displays the elapsed game time.

Game Loop
The main game loop handles events, updates object positions, checks for collisions, and updates the display.

End Game
When the game ends, the game over screen is displayed, showing the highest time and the player's time.

User Controls
Move the spaceship: W, A, S, D
Shoot lasers: SPACE
Shoot special lasers: X
Quit game: Q
FPS Control
The game maintains a frame rate of 60 frames per second using clock.tick(60).
