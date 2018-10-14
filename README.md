# I. Initiative
The program consists of two squares, one will be controlled by the user and one by the AI. The user must try to keep the square away from the enemy square. When the two squares come into contact the user will lose a life. If three lives are lost the game will be over. 

# II. Epics and User Stories

Epics 
- The user will control the user's square with a mouse
- The AI will control the enemy's square and will move towards the user's square
- When the two squares touch each other a life is lost 
- The game will need to take place in a canvas

Non-Functional Requirements
- The colour of the user's square should be green 
- The colour of the Enemy's square should be red 
- There will be a score displayed, the score will go up by one for every second the enemy square doesn't touch the user's square
- The user will have three lives

User Stories
- As a player I would like to be able to see my score on the screen. Also when the game is over I would like to see a highscore list, so that I can improve on my own score or try to beat people who played before me.
- As a player I would

How We Addressed The Requirements
A plan was set to have a score that the user can see and a highscore list that would come at the end of the game.  

# III. Genre

A game which will be played in a web browser 

# IV. Technical Details

Platform
HTML Browser

Programming Language/Enviroment
Java Script 

Programming Challenges
There were many challenges which I faced during this task:
- The project was asked to be done in notepad, debugging and solving the problem was an issue
- The enemy following the user's square, for a long time the enemy square would teleport to the user's position not follow it.
So it would always catch it
- Being able to implement the score feature
- Being able to implement a high-score list
- Being able to implement the three lives for the user

Constructing And Implementing My Code
Think of this as the method. How will you go about building your program?
Firstly, some research needed to be done to get the feel of how my code would look like. I used https://www.w3schools.com/ to help me understand further what was needed to be done. The program will be broken down in chunks, the canvas, the user's square and the enemy's square. Firstly, i will make the canvas, this is important because this is the area that the game is played in. Secondly, I will go about building the user square. Then I will try to add movement to the user's square by adding mouse movement, so when the mouse moves the user's square moves aswell. After, I will go onto build the enemy's square, here I will need this square to follow the user's square. After the game should restart when the two squares touch other. 

Algorithms

The algorithm in my program is to do with the enemy piece. When the user moves the game piece the AI will identify where the game piece is and will move towards it. When the enemy piece is on the left of the game piece the enemy piece will move right and when it is on the right of the game piece it will move left. when the enemy piece is above the game piece it will move down and it will move up if it is below it. This will move at a constant speed.

Coding Standards
Standard for the code you will be writting

# V. Research

This is the website I used for my research https://www.w3schools.com/. 
# VI. Project Management
Burndown Chart
file:///C:/Users/Toshiba/Pictures/burndown.PNG

Chart showing the completion of user stories over time

User Stories Tracking Chart (Which Stories Have Been Completed)
Table showing user stories with weighting, due date and completion state

Flowchart
Flowchart showing how the program will work

Functions
Descriptions of functions given on flowchart
