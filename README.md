
# Wumpus Game - AI Rule-Based System

## Overview
This project implements the **Wumpus Game**, an AI-driven game that simulates an agent navigating a cave environment filled with obstacles, treasure, and a dangerous Wumpus creature. The agent must explore the cave, deduce the location of hazards, retrieve the treasure, and exit safely. The project is implemented using **Jess (Java Expert System Shell)**, a rule-based AI programming language.

## Features
### Game Mechanics
- The agent navigates a **4x4 cave grid** starting from Room[1,1].
- The cave contains **pits, treasure, and a stationary Wumpus**.
- The agent has **a single arrow** to eliminate the Wumpus.
- The agent must use perceptual clues (stench, breeze, glitter) to navigate safely.
- The game follows logical **rules and AI-based decision-making**.

### Tasks Implemented
#### 1️ **Enhancing the Hunter's Reasoning Ability**
- The agent can **deduce** the exact location of the Wumpus and pits instead of general guesses.
- Implemented **rule-based inference** using Jess queries and rules.

#### 2️ **Introducing a New Goal: Killing the Wumpus**
- Added an action to **shoot the Wumpus** if the agent has arrows.
- Modified logic to ensure the **Wumpus remains dead** after being shot.
- Adjusted agent goals to include **retrieving gold and killing the Wumpus** before exiting.

#### 3️ **Improving the Hunter’s Navigation Ability**
- Implemented pathfinding logic to allow the agent to **move to a specified location efficiently**.
- Enhanced decision-making for avoiding risky paths while optimizing movement.

#### 4️ **Allowing the Hunter to Choose the Best Action**
- Implemented **decision-making logic** to prioritize actions based on risk and reward.
- Created a system to assess available moves and choose the **optimal strategy**.

## Technologies Used
- **Programming Language:** Jess (Java Expert System Shell)
- **AI Techniques:** Rule-based reasoning, inference, uncertainty handling

## Installation and Setup
1. Install **Jess** (Java Expert System Shell) from: [Jess Official Site](http://www.jessrules.com/)
2. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/Wumpus-Game.git
   ```
3. Navigate to the project directory and run the Jess engine with the `.jess` files.

## How to Run the Project
1. Open **Jess** in your terminal or command prompt.
2. Load the Wumpus World environment:
   ```lisp
   (batch "JessWumpus/ww.jess")
   ```
3. The agent will start navigating the cave based on the predefined rule-based logic.



