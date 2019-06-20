# Installation Instructions
Make Sure that your Device has OpenGL Graphics installed. Open the terminal in the current directory and compile the game using the following command : 

```g++ chessinterface.cpp -lglut -lGL -lGLU```

And now you can execute the game using the command :  

```./a.out```

# GLChess
A Chess program using OpenGl written entirely in C++
*(Python has been used to write large amounts of c++ openGL commands which will be addressed later)*

This project was made as an academic project during the second year of the college.

This is how it looks

![Demo](https://media.giphy.com/media/f6IVaSWY3YqcWzZULL/giphy.gif)

## Grapical interface
As mentioned before we made it using openGL 
Drawing the pieces in openGL is advised using texture mapping as its much more effecient but as we were on tight schedule and getting bugs , we had to find a loophole.Also the structure of our code could allow us to try such a method without much delay in execution.

PNG_to_pixelmap.ipynb uses python file handling as well as Pillow Image library to read the images and produce the C++ files by printing GL c++ commands that produce the pieces.

## Running the game
It is important to run a program to check all possible legal moves which requires analysis into the rules of chess
As far as the AI is concerned , it uses a evaluation function which evaluates the cost of state of board after every move and then uses a minimax tree along with alpha beta pruning to find the best possible move.

### Possible updates
1. Parallel Processing with Iterative Deepening to improve efficiency.
2. A graphical interface menu to make it more user friendly.

Please feel free to suggest improvements

