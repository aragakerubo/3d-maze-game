# 3D Maze Game

This project is a simple 3D maze game using SDL2 and raycasting. The goal is to navigate through a maze with the ability to rotate and move the player, avoiding collisions with walls.

## Table of Contents

-   [Requirements](#requirements)
-   [Installation](#installation)
-   [Compilation](#compilation)
-   [Running the Game](#running-the-game)
-   [Controls](#controls)
-   [Project Structure](#project-structure)
-   [Future Enhancements](#future-enhancements)

## Requirements

-   Ubuntu 14.04 LTS
-   gcc 4.8.4 or higher
-   SDL2 library

## Installation

### Install SDL2

```bash
sudo apt-get update
sudo apt-get install libsdl2-dev
```

## Compilation

Clone the repository and compile the code using the provided Makefile.

```bash
git clone https://github.com/aragakerubo/3d-maze-game.git
cd maze-project
make
```

## Running the Game

After compiling, you can run the game with the following command:

```bash
./maze_game
```

## Controls

-   **Left Arrow**: Rotate left
-   **Right Arrow**: Rotate right
-   **W**: Move forward
-   **S**: Move backward
-   **A**: Move left
-   **D**: Move right
-   **ESC**: Quit the game

## Project Structure

```
maze-project/
├── src/
│   ├── game.c
│   ├── main.c
│   ├── raycasting.c
│   ├── utils.c
├── include/
│   ├── game.h
│   ├── raycasting.h
│   └── utils.h
└── images/
└── README.md
└── Makefile
```

-   `src/`: Contains all source files
    -   `main.c`: Initializes SDL2, creates the window and renderer, and runs the main game loop.
    -   `game.c`: Contains the main game functions, including initialization, event handling, updating, and rendering.
    -   `raycasting.c`: Contains the raycasting functions to render the 3D maze.
    -   `utils.c`: Contains utility functions for player movement.
-   `include/`: Contains all header files
    -   `game.h`: Header file for game-related definitions and function prototypes.
    -   `raycasting.h`: Header file for raycasting-related function prototypes.
    -   `utils.h`: Header file for utility function prototypes.
-   `Makefile`: Build configuration
-   `images/`: Contains images used for textures and other graphics in the game.

## Tasks

### Task 0: Walls

-   Create a window with SDL2.
-   Use raycasting to draw walls on the window.
-   The color of the walls must be different from the color of the ground/ceil.
-   Provide a way to modify the map in your code to see if it works after recompiling it.

### Task 1: Orientation

-   Draw a different color depending on the orientation of the walls.
-   Draw walls facing NORTH and SOUTH in a different color from walls facing EAST and WEST.

### Task 2: Rotation

-   Provide a way to rotate the camera during the execution (e.g., using arrow keys or mouse).

### Task 3: Move

-   Provide a way to move the camera during the execution (e.g., using `W`, `A`, `S`, `D` keys).

### Task 4: Ouch!

-   Handle collisions of the player with the walls.
-   The player must not be able to enter walls.

### Task 5: Parser

-   Implement a parser to get the map from a file.
-   Define the standards of your map (e.g., character for a wall, character for nothing).

### Task 6: Draw the Map

-   Draw the map on the window.
-   Provide a way to enable/disable it during the execution.
-   Include the player’s line of sight in the map.

### Task 7: Coding Style + Documentation

-   Ensure the code fits the Holberton School coding style.
-   Ensure the code is well-documented.

### Task 8: Textures

-   Add textures on your walls.

### Task 9: Multi-task

-   Handle multiple events on the same frame (e.g., move in several directions and rotate at the same time).

### Task 10: Ground Textures

-   Add textures on the ground and/or on the ceiling.

### Task 11: Weapons

-   Add weapon textures.

### Task 12: Enemies

-   Add enemies to the game.

### Task 13: Make it Rain

-   Add rain and a possibility to stop/start the rain with a key.

### Task 14: Extra Option

-   Get creative! Add shadows, special lighting, etc.

## Future Enhancements

-   Add textures for walls, floors, and ceilings.
-   Implement a map parser to load the maze from a file.
-   Add collision detection to prevent the player from walking through walls.
-   Implement enemy entities and player weapons.
-   Add weather effects like rain and fog.
-   Improve graphics and add shadows and special lighting effects.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Contributing

Feel free to fork the repository and submit pull requests. Contributions are always welcome!

## Credits

-   SDL2 tutorials: [SDL2 tutorials](https://lazyfoo.net/tutorials/SDL/)
-   Raycasting tutorial: [Alternative Raycasting Tutorial](https://lodev.org/cgtutor/raycasting.html)
