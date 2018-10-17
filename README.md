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
- The size of both squares should be the same

User Stories

- (1) As a player I would like to see the the canvas and the 2 squares 
- (2) As a player I would like to see my square move to the location I have chosen
- (3) As a player I would like to see the enemy piece move towards the game piece
- (4) As a player I would like the game to stop once the 2 squares come into contact 
- (5) As a player I would like to be able to see my score on the screen
- (6) As a player I would like to see a highscore list 
 

How We Addressed The Requirements
A plan was set to have all the requirments that were asked for. Having a canvas and 2 squares were important, so this was a good place to start.   

# III. Genre

A reaction game

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
Firstly, some research needed to be done to get the feel of how my code would look like. https://www.w3schools.com/ was used to help understand further what was needed to be done. The program will be broken down in chunks, the canvas, the user's square and the enemy's square. Firstly, the canvas will be made, this is important because this is the area that the game is played in. Secondly, I will go about building the user square. Then I will try to add movement to the user's square by adding mouse movement, so when the mouse moves the user's square moves aswell. After, I will go onto build the enemy's square, here I will need this square to follow the user's square. After the game should restart when the two squares touch other. 

Algorithms
When the user moves the mouse the game piece will move the enemy piece will listen out to the coordinates and will move towards it. When the enemy piece is on the left of the game piece the enemy piece will move right and when it is on the right of the game piece it will move left. When the enemy piece is above the game piece it will move down and it will move up if it is below it. This will keep happening until the 2 squares contact each other, once this happens the game will stop. 

Coding Standards

- In this program all the curly brackets are opened at the same place
- All the code is indented the same 
- 


IDE 


An IDE was not used in the creation of this program, as the program was created in notepad. 




# V. Research

https://www.w3schools.com/. 


# VI. Project Management
Burndown Chart

![Burndown](https://i.imgur.com/V2JQ8T8.png)


Chart showing the completion of user stories over time
![User Stories tracking Chart](https://i.imgur.com/kloPwQO.png)


Flowchart


![Flowchart](https://i.imgur.com/7WpAWUJ.png)



Functions
Descriptions of functions given on flowchart


Here is the code which displays the components

The first image shows the creation of the compnents and the second image places the components into the canvas.






