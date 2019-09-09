# Lights Out Game App
Lights Out Game is a complete browser-based game to test a user's logic. The game is implemented in *React*.

## Table of Contents

* [Game Rules](#game-rules)
* [Game Screenshots](#game-Screenshots)
* [Game Functional Requirements](#game-functional-requirements)
* [Game Design](#game-design)
* [How to Run and Play the Game](#how-to-run-and-play-the-game)
* [Credits](#credits)
* [Technologies Used](#technologies-used)
* [Acknowledgement](#acknowledgement)
* [Future features](#future-features)

### Game Rules
Lights Out is a logic/puzzle game, played on a grid of individuals lights, which can either be lit or unlit.

Each turn:

- The player can click on a cell to toggle that light, but it also toogles the light above it, to the left of it, or the right of it, and below it.
- Cells on edge or in the corner won't flip as many lights, since they are missing some neighbours.


The puzzle is won when all all of the lights are turned off.


### Game Screenshots
**Fig 1. Initial game screen**

![alt memory](/img/initial_game.png)

**Fig 2. Winning game**

![alt modal](/img/win_game.png)



### Game Functional Requirements
The functionalities to be implemented are:

1. Create a ***board of cells*** that randomly lights the cells.
2. Handle user ***click*** interactions to ***flip the cells***. This should flip the clicked cell and the cells around it.
3. Control the ***winning condition***: When the game is won, the board should not be shown, but a simple "You won" message should show in its place.


### Game Design
The application consists of three components

* **App.js**: This is a very simple component. It just renders the Board component.

* **Board.js**: This is the central component of the game. It holds the state that represents the in-memory grid of true/false for lights on/off.
* **Cell.js**: This component simply render a *<div>*, where the CSS classes indicates whether this cell is lit or unlit. This is what the user clicks on - but it will need to call a function it receives from the Board, since that will need to update the State.



### How to Run and Play the Game
- **Run:** Click [Here](https://lpinzari.github.io/lights-out-game/) to play the LivePreview of the Game hosted on GitHub. If you want to run the game *locally* on your computer,you can download the files from this repository or clone them.
    - **Download**: Click the <code>Clone or download</code> green button and you'll get the *Project Zip* file. When your download finishes, unzip the file and run the command <code>npm install</code> and <code>npm start</code>
    - **Clone**: type into your terminal the following <code> $ git clone https://github.com/lpinzari/lights-out-game.git</code>.



### Credits
- For styling the *header title* Javascript function was used from [https://codepen.io/Trinca/pen/NAvpWa](https://codepen.io/Trinca/pen/NAvpWa)
- React tutorial [https://reactjs.org/tutorial/tutorial.html](https://reactjs.org/tutorial/tutorial.html)
- To deploy React Front end app on GitHub pages [https://codeburst.io/deploy-react-to-github-pages-to-create-an-amazing-website-42d8b09cd4d](https://codeburst.io/deploy-react-to-github-pages-to-create-an-amazing-website-42d8b09cd4d)

### Technologies Used
- **HTML** | **CSS** | **React**


### Acknowledgement
I'd like to thank the GA's instructors for the useful advices.

### Future features
- Responsiveness on small devices.

#### Author
Ludovico Pinzari

#### License
MIT
