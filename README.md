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

There are 6 videos below, each showing a different feature/example:
1) ![All commands](https://github.com/TommyStar123/Chess/assets/67210363/87f58edf-64a8-40a8-8049-b22657a41a81)

2) ![Castling on both sides](https://github.com/TommyStar123/Chess/assets/67210363/e2909935-5c37-403e-be95-a9dc8705531a)
   
3) ![Stalemate](https://github.com/TommyStar123/Chess/assets/67210363/e163978f-c531-40a1-a4f2-669090f7116a)

4) En Passant
https://github.com/TommyStar123/Chess/assets/67210363/45e03456-d58d-4604-a105-7381a9290c71
  
5) Pawn Promotion using computers
https://github.com/TommyStar123/Chess/assets/67210363/2fca6d00-e9c8-44c1-855a-ac2bca8be19f

6) Regular Checkmate
https://github.com/TommyStar123/Chess/assets/67210363/30055530-3a34-4e9d-8f63-9a2599ff9b3d







