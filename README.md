# Cops and Robbers Simulation

A console-based C++ simulation of a pursuit across a 10x10 city grid. The program places jewels, robbers, and a police unit on the map, then advances the simulation through 30 rounds of movement and interaction.

## Overview

The simulation models a small city containing:

- Four robbers with individual positions and greed states
- One police unit that moves through the city
- Forty-seven jewels placed at randomly selected locations
- Robber movement across the grid in eight possible directions
- Loot collection and loot division when active robbers meet
- A printed grid after the initial setup and after each round

The project demonstrates object-oriented design, templates, header/source organization, arrays, and randomized simulation logic in C++.

## Grid Legend

| Symbol | Meaning |
| --- | --- |
| `J` | Jewel |
| `r` | Robber during initial placement |
| `1`-`4` | Individual robbers during the simulation |
| `R` | Robbers sharing a location |
| `p` | Police unit |
| Blank space | Unoccupied location |

## Build and Run

### Requirements

- A C++ compiler with C++11 or later support
- A terminal or command prompt

### Compile

From the project directory, run:

```bash
g++ -std=c++11 -Wall -Wextra main.cpp city.cpp jewel.cpp police.cpp -o cops_and_robbers
```

### Run

```bash
./cops_and_robbers
```

The simulation prints the initial city grid, movement details for each round, and the updated grid for all 30 rounds.

## Project Structure

| File | Purpose |
| --- | --- |
| `main.cpp` | Initializes the simulation and runs the rounds |
| `city.h` / `city.cpp` | Defines and manages the 10x10 city grid |
| `robber.h` / `robber.hpp` | Defines the templated robber and movement behavior |
| `police.h` / `police.cpp` | Defines police movement and arrest-related behavior |
| `jewel.h` / `jewel.cpp` | Defines jewel coordinates and values |

## Project Brief

The original assignment specification is available in [Final Programming Project.pdf](Final%20Programming%20Project.pdf).

## Contributors

- Parsa Divanbeigi
- Raphael Seymour
