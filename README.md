# Tic Tac Toe - Weekend Lab

**Objective:** Build a tic-tac-toe game in HTML, CSS, and JavaScript.


This week, we've been learning about working with conditionals and loops, as well as writing functions. We've also learned about the structure of the DOM and how we can interact with it using CSS and JavaScript. We've looked at Bootstrap's CSS library and at jQuery, a JavaScript library for front end web development.

For your first weekend lab, we'll be making a tic-tac-toe game using your knowledge and skills from this week.

## Baseline Requirements
* Users should be able to click on any empty box to make a move.   
* Every move should alternate between marking an `X` and `O` (the two players).  
* A user should not be able to claim a box that has already been claimed for `X` or `O`.
* Users should be able to click a "reset" button to clear all `X`'s and `O`'s from the board and restart the game.


## Further Challenge Ideas

* Display a message to indicate which player's turn is about to be played (`X` or `O`).    

* If a player wins, show a message with the mark of the winner.
    <details><summary>Hint: checking for winner</summary><p>Determine all the winning combinations. Check those combinations against the board contents after every move.</p></details>  
    <details><summary>Hint: showing a message</summary>Try an `alert`. For an extra challenge, put a message directly onto the page using jQuery!</details>

* If the board fills up before anyone wins, show a message that it was a draw.

* Display separate colors for `X`'s and `O`'s. <details><summary>Hint</summary><p>Use jQuery to add a CSS class to the square when a player makes a move.</p></details>


* Creatively style your tic-tac-toe site!

## Suggested Workflow

**Set up repository, files, and basic structure.**

1. Fork this repository to create a copy on your GitHub account.

1. Clone the tic-tac-toe repository from *your GitHub account* into your `wdi` folder to create a local copy on your computer.

2. Use `index.html` as your starting point on this project. There is already some starter code in `index.html`, `css/style.css`, and `js/app.js`.

1. Make sure that jQuery and Bootstrap's CSS are linked in your `index.html`. Also link your custom CSS and JavaScript files to your `index.html`.

3. Test that your CSS and JavaScript files are linked to your `index.html` by adding an alert to `app.js` and opening `index.html` in the browser. You should see part of an empty tic-tac-toe game board, and you should also see your alert message pop up.

1. Use Bootstrap's grid system to create the rest of the empty tic-tac-toe game board. The empty board should look like this:

    <img src="board.png" width="300px" alt="empty tic tac toe board">

1. Add a reset button below the board.

**Gameplay:**

1. Use the `$()` jQuery function with CSS selectors to locate each of the DOM elements your user will click. Try this in your console to make sure your selection works. Set up variables for them in your `app.js`.

1. After you find the elements, use `.on` to set up a simple `click` event listener for those elements. Start by having your event listener function just log a message that the element was clicked.  

1. Most of your game logic will happen when a user clicks one of the boxes on the board.


  **Here are some hints and tips:**
  	<details><summary>Track Turns</summary><p>You need to keep track of whose turn it is. This will be important when deciding whether to draw an `X` or an `O`. Try storing the turn as a variable.</p></details>
	<details><summary>Whose Square?</summary><p>You'll need a way for your code to check whether a square is empty. When a square is claimed, use jQuery to change something about the square's DOM element. Then you can check that feature of the square later! Test your ideas in the console.</p></details>
	<details><summary>Reset Everything</summary><p>Your reset button should change the board back to its initial configuration. Make sure you empty all the squares and reset all other variables to their starting values.</p></details>
  	<details><summary>Detect a Draw</summary><p>The game can end when someone wins or if the board is full. How can you check whether the board still has space for the players to move?</p></details>
  	<details><summary>Winner!</summary><p>Separate your code that checks for a winner into a separate function. You'll need to call this function often. When?</p></details>

## Submission

* As you make code changes, frequently commit and push to GitHub.
* Once you've finished the assignment and pushed your work to GitHub, make a pull request from your fork to the original repo.
