---
layout: page
title: Snek
description: A playable snake game implemented in C, practicing core concepts of systems programming.
importance: 4
category: School Projects
related_publications: false
---

### Overview

[Snek](https://inst.eecs.berkeley.edu/~cs61c/sp23/projects/proj1/) is a classic snake game implemented as a part of the CS 61C project. The objective of the game is to navigate a snake through a grid, consuming fruits to grow longer while avoiding collisions with walls and the snake's own body. This project focuses on C programming, memory management, and struct manipulation.

---

### Project Requirements

**Setup and Initial State:**
- The game board consists of walls, empty spaces, fruits, and one or more snakes.
- Each snake is represented by a series of characters indicating its direction and position.
- Snakes move in the direction of their heads, growing longer when they consume fruits.

**Game Mechanics:**
- Implemented functions to manage the game state, including creating the default state, freeing allocated memory, and printing the board.
- Developed logic to update the game state, handling snake movements, collisions, and fruit consumption.
- Ensured proper memory management and efficient board loading from a file.

**Tasks and Implementations:**
1. **create_default_state:** Initialized the game board with a predefined layout and placed a snake and a fruit.
2. **free_state:** Freed all dynamically allocated memory for the game state, preventing memory leaks.
3. **print_board:** Printed the current state of the game board to a specified file.
4. **update_state:** Updated the game state based on snake movements, collisions, and fruit consumption.

---

### Implementation

**Structs and Memory Management:**
- Utilized `game_state_t` and `snake_t` structs to manage the game board and snake information.
- Managed dynamic memory allocation for the game board and ensured efficient memory usage.

**Game Logic:**
- Implemented helper functions to determine snake characteristics and movements.
- Developed functions to update the snake's head and tail positions, manage collisions, and handle fruit consumption.

**File Handling:**
- Implemented `load_board` to read the game board from a file, handling boards of varying sizes and shapes.
- Developed `initialize_snake` to create and initialize snake structs based on the game board.

**Gameplay Integration:**
- Combined all functions to create a working snake game that updates the board with each time step.
- Allowed for interactive gameplay and automated testing of various game scenarios.

---

### Features

**Basic Gameplay:** \
Implemented the core mechanics of the game, including snake movements, fruit consumption, and collision detection.


**Memory Management:** \
Ensured efficient memory allocation and deallocation, preventing leaks and optimizing performance.


**Interactive Gameplay:** \
Developed an interactive version of the game for users to play and test their implementations.


---

### Conclusion

The Snek project provided hands-on experience in C programming, memory management, and game development. By completing this project, I gained valuable skills in handling dynamic memory, implementing complex game logic, and managing data structures in C.

---

