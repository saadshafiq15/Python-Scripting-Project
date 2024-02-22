# Game Directory Processor

## Overview

This project is designed to process game directories within a specified data directory. It assumes that the data directory contains numerous files and subdirectories, with our primary interest being in directories related to games. Each game is stored in a directory marked with the name "game," and within each game directory, there is a single `.go` file that needs to be compiled before running.

The project aims to perform the following tasks:

1. Identify game directories within the specified data directory.
2. Create a new directory for processed games.
3. Copy the contents of each game directory into the new games directory, removing the "game" suffix from each directory.
4. Generate a `.json` file containing information about each game.
5. Compile the code in each game directory.
6. Run the compiled code for each game.

## Assumptions

- The project assumes that the relevant game directories are labeled with the name "game."
- Only the game directories within the specified data directory will be processed.

## Usage

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/game-directory-processor.git
   cd game-directory-processor

2. Confirm file structure:

    game-directory-processor/
    ├── data/
    │   ├── game1/
    │   │   ├── game1.go
    │   ├── game2/
    │   │   ├── game2.go
    │   └── ...

3. Run the script:

   python process_games.py <data> <target_folder_name>

## Dependencies

- Python 3.XX

