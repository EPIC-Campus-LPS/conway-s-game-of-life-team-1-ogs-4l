# Lab 1: Conway's Game of Life
## Objective: Complete the program to implement Conway's Game of Life
1. Create a GitHub account using your LPS email address and connect it to IntelliJ under the VCS menu.
2. Connect your GitHub account to the GitHub Classroom via the Lab 1.1: Git & GitHub Fundamentals assignment in Google Classroom
3. Pull the GameOfLife GitHub Repository from GitHub Classroom.
4. Research Conway's Game of Life with the provided links.
    1. You will be asked to write about your findings in your README.
5. Use a GitHub repository for your team to develop your code.
    1. At the end of this project, there should be multiple commits. Do not just create your project on one machine and upload it to a shared GitHub when you are done.
6. Implement the *oneGeneration()* method in the *LifeModel.java* file as described below.
7. Complete the questions on the README document.
8. Before you submit, be sure to consult the Style Guidelines for the course and for this project.

## Conway's Game of Life
This is not really a game.  It is an implementation of a cellular automata that John H. Conway chose to call the “Game of Life.” The computer simulation is of the life and death events of a population of bacterial organisms.  This program will determine the life, death, and survival of bacteria from one generation to the next, assuming the starting grid of bacteria is considered generation zero.  Sometimes the outcome is that all organisms die.  Other times they end up in a static or oscillating world.  Other times, they form organisms that generate new life forms that glide across the screen. 
### Links to Research
- [http://www.math.com/students/wonders/life/life.html](http://www.math.com/students/wonders/life/life.html)
- [https://en.wikipedia.org/wiki/Conway%27s_Game_of_Life](https://en.wikipedia.org/wiki/Conway%27s_Game_of_Life)
- Try out this cool simulation: [https://bitstorm.org/gameoflife/](https://bitstorm.org/gameoflife/)

## Game Specifications
The sizeof the grid is set to a square 60 x 60.  Different sized grids produce different results.

## Model-View-Controller Framework
This application uses the Model-View-Controller(MVC) design framework. You don't have to worry too much about it, since the *LifeView.java* and *LifeController.java* classes are already written for you. If you want some more information on MVC, here are some links to check out.
- https://www.geeksforgeeks.org/mvc-framework-introduction/#
- https://en.wikipedia.org/wiki/Model%E2%80%93view%E2%80%93controller

## Starter Code
1. You are provided with a data file that describes an initial population of the life grid, life100.txt.  Use these file to test your program and make sure it is working correctly.  Data files for 4 other really interesting patterns are contained in the program folder, also run your program using them as input.  (blinker_lif.dat, glgun13_lif. dat, penta_lif. dat, tumbler_lif. dat)
    1. The first line of the file will contain the number (N) of bacteria locations in the file.
    2. What follows are N **pairs of data**, one pair of numbers per line. 
	3. The first value of each line indicates the row location while the second value on the line indicates the column location. 
	4. The data file values are given as:  0 <= Row < 60 and 0 <= Col < 60.
2. This project follows the **Model-View-Controller model**.  You are provided with the Controller (main program), **Life.java** and the View, **LifeView.java**.  You are also provided with a skeleton Model component, **LifeModel.java**.  Each cell is an object, defined by the **LifeCell class**. The starter code will provide a GUI for your to interact with; your coding will be done in the model component.
3. Your task is to implement the *oneGeneration()* method.

## oneGeneration()
Your *oneGeneration()* method must implement the rules of Conway's Game of Life as described below. **Complete the "helper methods" given to keep your code simple and organized.** The method *oneGeneration()* will be called automatically over and over once the Run button has been clicked to advance from generation to generation. It can also be paused, resumed, or stepped under user's control.

## Extensions
- **Enhance** your now working Life program!  Add in color, age, wrap-around grid, etc…  Be sure to talk about/explain your enhancement in your reflection and include a **video** demonstrating your additions

## Testing
A sample run output for **generation 5** is given below.  Note, these are the correct answers if you use the provided data file "_life100.txt_".  If you let life run for a long time, it will oscillate between the last 3 patterns.  There are actually 6 patterns as the line of three keeps switching.![GameOfLifePicture1 (3)](https://github.com/gormes-EPIC/GameOfLife/assets/134316348/1b1e4ff8-6c15-4851-be86-93fbadae919a)
![GameOfLifePicture1 (2)](https://github.com/gormes-EPIC/GameOfLife/assets/134316348/fb3cde51-def1-4c9c-a9c4-0496139dfca9)
![GameOfLifePicture1 (1)](https://github.com/gormes-EPIC/GameOfLife/assets/134316348/a4ff0355-2bbd-497a-b9d5-d9871519fca5)

## Deliverable
- Your Java project with a completed *LifeModel.java* file. Adhere to the Style Guidelines.
- Completed README.md file that answers the provided questions.

##### Sources
This starter code was created by Kimberly Jans. Original solution with graphics based on work by Roger Frank from Ponderosa High School in Parker, CO
