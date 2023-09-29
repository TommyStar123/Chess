# Chess
This project was a full recreation of chess using C++, displayed using xWindows graphics. 

# Project Design
Before beginning the project, a UML was created to plan out the design and structure of the classes. This can be seen below:

![image](https://github.com/TommyStar123/Chess/assets/67210363/ae64115d-c039-4c65-8345-13137c29ceec)

As seen in the UML, multiple object oriented design principles such as polymorphism for the chess pieces (inheriting from the Piece abstrac tclass) and design patterns such as the Model-View-Controller pattern (used for ensuring the piece movement was reflected on the graphical and text display) were used in the project. The RAII idiom was also ahered to throughout the code, through the use of shared and smart pointers. 



