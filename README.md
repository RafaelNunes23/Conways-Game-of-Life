# Conway's Game of Life

A terminal-based implementation of **Conway's Game of Life written in C**.

This project was developed as part of my university studies to practice C programming concepts such as dynamic memory allocation, matrices, file handling, and simulation algorithms.

## How It Works

The program reads an initial grid from a text file and simulates Conway's Game of Life for a selected number of generations.

Each cell follows the classic rules:

* A live cell survives if it has 2 or 3 live neighbors.
* A live cell dies if it has fewer than 2 or more than 3 live neighbors.
* A dead cell becomes alive if it has exactly 3 live neighbors.

During the simulation, the terminal displays the current generation and the number of live and dead cells.

The simulation can also be paused and resumed by pressing **Space**.

## Features

* Conway's Game of Life simulation
* Custom initial grid loaded from a file
* Adjustable number of generations
* Adjustable simulation speed
* Live and dead cell counter
* Colored terminal visualization
* Pause and resume using the Space key
* Dynamic memory allocation

## Project Structure

```text
conways-game-of-life/
│
├── src/
│   └── conways_game_of_life.c
│
├── examples/
│   └── example1.vid
│   └── example2.vid
│   └── example3.vid
│   └── example4.vid
│   └── example5.vid
│   └── example6.vid
│   └── example7.vid
│
└── README.md
```

## Input File

The initial grid is loaded from a text file.

The first line contains the number of rows, the second line contains the number of columns, followed by the grid using `0` for dead cells and `1` for live cells.

Example:

```text
5
5
00000
00100
00100
00100
00000
```

## Compilation

Using GCC on Windows:

```bash
gcc src/conways_game_of_life.c -o conways_game_of_life.exe
```

## Usage

Run the program:

```bash
conways_game_of_life.exe
```

Then provide:

1. The path to the initial configuration file
2. The number of generations
3. The execution speed in seconds

During the simulation, press **Space** to pause or resume.

## Technologies

* C
* Windows Console
* Standard C Library

## Author

University project developed for programming practice.

