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


Firstly, some research needed to be done to get the feel of how my code would look like. https://www.w3schools.com/ was used to help understand further what was needed to be done. The program will be broken down in chunks, the canvas, the user's square and the enemy's square. Firstly, the canvas will be made, this is important because this is the area that the game is played in. Secondly, I will go about building the user square. Then I will try to add movement to the user's square by adding mouse movement, so when the mouse moves the user's square moves aswell. After, I will go onto build the enemy's square, here I will need this square to follow the user's square. After the game should restart when the two squares touch other. 

Algorithms


The game will start when the page has loaded, when the user moves the mouse the game piece will move the enemy piece will listen out to the coordinates and will move towards it. When the enemy piece is on the left of the game piece the enemy piece will move right and when it is on the right of the game piece it will move left. When the enemy piece is above the game piece it will move down and it will move up if it is below it. This will keep happening until the 2 squares contact each other, once this happens the game will stop. 

# Coding Standards

- In this program all the braces were placed at the same position in the code, this is shown in the image below. 

![](https://i.imgur.com/Y1VO9vg.png)


- All the code is indented inside a new block of code


![](https://i.imgur.com/x02pLLd.png)

- Camel casing was used when creating new variables, as shown below


![](https://i.imgur.com/a3mf42d.png)


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


1. Display user's piece, enemy piece and canvas 
 
Here is the code which displays the canvas content and colour of the border. 
    
    canvas {
    border:1px solid #d3d3d3;
    background-color: #f1f1f1;
    }
    
The next line of code just get the canvas and can give it things like width, height and style. 
    
    
    canvas : document.createElement("canvas")
    
The next step was to create the components. The game piece is the component that the user controls and the enemy piece is the component the AI controls. When creating the components some specification would need to be given.  The Width, height, colour and the x and y coordinates.
    
    myGamePiece = new component(50, 50, " lightgreen", 100, 100); 			 
    myEnemyPiece = new componentEnemy(25, 25, "red", 0, 0); 
Functions needed to be created to display the components into the canvas. 


2. Enemy's square will follow the user's square

Next the AI will need to locate where the game piece and travel to that location.

    
		if (myGamePiece.x < myEnemyPiece.x) {			
		myEnemyPiece.x = myEnemyPiece.x -1		
		}						
		else {
		myEnemyPiece.x = myEnemyPiece.x +1		 
		}
The code above will get the enemy piece to move right or left depending on where the game piece is by following its x coordinates.

		if (myGamePiece.y < myEnemyPiece.y) {			 
		 myEnemyPiece.y = myEnemyPiece.y -1
		 }
		 else {
		 myEnemyPiece.y = myEnemyPiece.y +1
	 	}
The code above will get the enemy piece to move up or down depending on where the game piece is by following its y coordinates.
   
3. The user's square will move in the direction they have chosen
   
Now the user's square will listen out for mouse movement from the user. The code below shows what will make this happen. 
   
    window.addEventListener('mousemove', function (e) { 			 
         	   myGameArea.x = e.pageX;
            	myGameArea.y = e.pageY;
        })
        
4. Stop the game when game piece has been caught

Lastly, when the two pieces come into contact the game must stop and a game over message must be displayed. Unforunately I did not include lives in this game. 

    if ( (myEnemyPiece.x == myGamePiece.x) && (myEnemyPiece.y == myGamePiece.y)  ){
		  alert("GAME OVER - You've been caught");
    document.location.reload();
		  }
    
The code will tell the program to stop once the x and y coordinates are all at the same location, it will then reload the page after a game over message. 




# VI. Evaluation 

For me this project was a success, I have managed to create a fully functional program in 2 weeks. This program has all the main requirements that allows the user to play the game. Getting the user's piece and enemy piece to work the way they were suppose to gave me great satisfaction, this is because alot of reasearch and understanding went into to finding out how they would work. 

The game was created in notepad which I found very difficult, I have a basic understanding of programming but coding without the use of an IDE was a first for me. Coding without the use of an IDE is challenging because there wasn't an error message to tell you where you have gone wrong or what syntax the code doesn't understand. To make this right I had to run it in a browser and use the console there to find my mistakes and correct it. This was very time consuming. 

I would have liked to add a score and lives to the game but unfortunately I ran out of time. With more time I would have like to add many more features. 


     
   
    


    
    
    
    
    






