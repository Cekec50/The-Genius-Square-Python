# The Genius Square

This project is a Python-based implementation of the board game "The Genius Square". It features a graphical user interface (GUI) and includes AI algorithms to solve the puzzle, allowing for both player versus player and player versus AI gameplay. This was developed as a Bachelor's Thesis Project.

## Overview

The Genius Square is a puzzle game where the objective is to fit a set of nine unique wooden shapes onto a 6x6 grid. At the start of each game, seven "blocker" pieces are placed on the grid at positions determined by rolling a set of seven dice. The player must then arrange the nine shapes to fill all the remaining empty squares on the board.

This digital version of the game provides a platform to play the game and also serves as a framework to explore and compare different AI-based puzzle-solving algorithms.

## Tech Stack

*   **Language:** Python
*   **Libraries:**
    *   [Pygame](https://www.pygame.org/): For creating the graphical user interface and handling user interactions.

## Features

*   **Game Modes:**
    *   **Player vs. Player:** Two players can compete to see who can solve the puzzle faster.
    *   **Player vs. AI:** A single player can challenge an AI opponent.
*   **AI Opponents:** The AI can use one of three different algorithms to solve the puzzle, each representing a different difficulty level:
    *   **Easy (Brute Force):** A straightforward approach that tries all possible combinations. It's fast but not very strategic.
    *   **Intermediate (DFS):** Uses a Depth-First Search algorithm for a more strategic, but slower, approach.
    *   **Hard (Best-First Search):** Employs a Best-First search algorithm with heuristics for an even more advanced and strategic solution, but it is the slowest.
*   **Interactive Gameplay:**
    *   A user-friendly GUI built with Pygame.
    *   Randomized "blocker" placement by simulating dice rolls.
    *   Simple controls for placing and rotating the puzzle pieces.
    *   A timer to track how long it takes to solve the puzzle.

## Getting Started

Follow these instructions to get a copy of the project up and running on your local machine.

### Prerequisites

*   Python 3.x
*   pip (Python package installer)

### Installation

1.  Clone the repository to your local machine:
    ```bash
    git clone https://github.com/your-username/The-Genius-Square---Bachelor-s-Thesis-Project.git
    cd The-Genius-Square---Bachelor-s-Thesis-Project
    ```

2.  Install the required Python packages:
    ```bash
    pip install pygame
    ```

### Running the Application

To start the game, run the main Python script from the project's root directory:

```bash
python TheGeniusSquare.py
```

## Project Structure

The project is organized into the following files and directories:

*   `TheGeniusSquare.py`: The main entry point of the application. It handles the game loop, user interface, and event handling.
*   `Algorithms.py`: Contains the implementations of the AI puzzle-solving algorithms (Brute Force, DFS, Best-First Search).
*   `Classes.py`: Defines the primary classes used in the game, such as `Piece` for the puzzle shapes and `Node` for the search algorithms.
*   `ConstValues.py`: A collection of constant values used throughout the project, including colors, screen dimensions, and piece definitions.
*   `images/`: A directory containing the background images used in the game.

## Usage

1.  Launch the game by running `python TheGeniusSquare.py`.
2.  From the main menu, select either **Player vs. Player** or **Player vs. AI**.
3.  If you choose Player vs. AI, you will be prompted to select a difficulty level (Easy, Intermediate, or Hard).
4.  Click the **ROLL** button to randomly place the seven "blockers" on the grid.
5.  To place a piece, click and drag it from the right-hand panel onto the main grid.
6.  To rotate a selected piece, press the **SPACE** key or click the **ROTATE** button.
7.  The objective is to fill all the empty squares on the grid. The first player to complete the puzzle wins.
8.  You can quit the game at any time by clicking the **QUIT** button or closing the window.
