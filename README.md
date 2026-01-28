# Checkers Game using OOPS (C++)

## Author
**Jay Harish E**  
GitHub: https://github.com/JAY-HARISH-E
LinkedIn: www.linkedin.com/in/jay-harish-e-7115k


## Overview
This project is a console-based implementation of the classic **Checkers game** developed in **C++**.  
The main goal of the project is to demonstrate the practical use of **Object-Oriented Programming (OOP)** concepts such as encapsulation, inheritance, polymorphism, operator overloading, and dynamic memory management.

The game supports both **two-player mode** and **player vs computer mode**, providing an interactive gameplay experience through the terminal.

---

## Project Objectives
- To apply core **OOP principles** including encapsulation, abstraction, inheritance, and polymorphism.
- To implement **operator overloading** for cleaner and more readable code.
- To design a structured and manageable class architecture for the game.
- To develop a console-based Checkers game with:
  - Player vs Player mode
  - Player vs Computer mode

---

## Design and Implementation

### Class Structure
The project is organized using three main classes:

- **Board**
  - Manages the 8×8 game board
  - Handles piece placement, movement validation, and move execution
  - Implements operator overloading for easy board access and comparison

- **Player**
  - Represents a player (human or computer)
  - Handles move execution logic
  - Uses a simple AI strategy for computer moves

- **Game**
  - Controls the overall game flow
  - Switches turns between players
  - Detects game over conditions and declares the winner

---

## Object-Oriented Concepts Used

### Encapsulation
Each class manages its own data and exposes only the necessary methods required for interaction.

### Operator Overloading
The following operators are overloaded in the `Board` class:
- `()` → Access board elements like a 2D array  
- `<<` → Print the board directly using `cout`  
- `==` → Compare two board states

### Inheritance and Polymorphism
- A base class `PlayerBase` is created.
- The `Player` class inherits from `PlayerBase`.
- `playermove()` is declared as a **pure virtual function** in the base class and overridden in the derived class.
- This allows flexible handling of human and computer players using polymorphism.

### Dynamic Memory Management
Player objects are dynamically allocated and properly released using destructors to avoid memory leaks.

### Exception Handling
Exception handling is used to validate the selected game mode.  
If the user enters an invalid game mode, an exception is thrown and handled gracefully with an error message.

---

## Features
- Console-based user interface
- Player vs Player mode
- Player vs Computer mode
- Board printing using operator overloading
- Simple AI logic for computer player
- Input validation using exception handling

---

## How to Compile and Run

### Compile
g++ checkersheader.h checkers.cpp checkersmain.cpp -o out

## run 
.\out
