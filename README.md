# Chess
This project is a full recreation of chess using C++, displayed using xWindows graphics. All features, including En Passant, pawn promotion, and castling are implemented. 
Bonus features include computer bots of 3 difficulties and a visual display of the chess board.

## Project Design
Before beginning the project, a UML was created to plan out the design and structure of the classes. This can be seen below:

![image](https://github.com/TommyStar123/Chess/assets/67210363/ae64115d-c039-4c65-8345-13137c29ceec)

As seen in the UML, multiple object oriented design principles such as polymorphism for the chess pieces (inheriting from the Piece abstrac tclass) and design patterns such as the Model-View-Controller pattern (used for ensuring the piece movement was reflected on the graphical and text display) were used in the project. The RAII idiom was also ahered to throughout the code, through the use of shared and smart pointers. 

## Demo

The list of commands include: 
- _game <white player> <black player>_ - used to start a game between any of: human, computer1, computer2, computer3
  - The number beside the computer indicates a higher difficulty, with 1 being the lowest and 3 being the highest
- _resign_ - used to resign during the current player's turn during a game
- _move <origin square> <destination square>_ - origin and destination squares are specified through column (alphabetical letter) followed by row (number), ex. _move e7 e6_
- _setup_ - used to setup a board before starting a game; if a board has not been setup the game will use the default chess board with the typical black and white pieces on each side
    - Certain restrictions are required to exit setup mode:
        - Pawns can’t be at the end of the board and there must be 1 black King and 1 white King

Additional notes:
(_game_ and _setup_ can only be run while a game is currently not in progress)
( _resign_ and _move_ can only be run while a game is currently in progress)

As seen below, there are two visual displays of the chess board, both of which update after each move:
![image](https://github.com/TommyStar123/Chess/assets/67210363/1ac94e45-957b-4265-83ce-3e33747ab9eb)

The video below contains 6 examples:
- 0:00 - All commands
- 0:58 - Castling on both sides
- 1:49 - Stalemate
- 2:11 - En Passant
- 2:49 - Pawn Promotion using computers
- 3:29 - Regular Checkmate





