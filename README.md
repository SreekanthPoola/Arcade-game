# Classic Arcade Game Clone Project

## Table of Contents

- [Instructions](#instructions)
- [Contributing](#contributing)

## Instructions

Use this [rubric](https://review.udacity.com/#!/rubrics/15/view) for self-checking your submission.

Make sure the functions you write are **object-oriented** - either class functions (like `Player` and `Enemy`) or class prototype functions such as `Enemy.prototype.checkCollisions`. Also make sure that the keyword `this` is used appropriately within your class and class prototype functions to refer to the object the function is called upon.

Your **README.md** file should be updated with instructions on both how to 1. Run and 2. Play your arcade game.

For detailed instructions on how to get started, check out this [guide](https://docs.google.com/document/d/1v01aScPjSWCCWQLIpFqvg3-vXLH2e8_SZQKC8jNO0Dc/pub?embedded=true).

## Contributing

This repository is the starter code for _all_ Udacity students. Therefore, we most likely will not accept pull requests.

## I followed the following steps to complete the project

###Cloning the Project
- After following the instructions, I got a GitHub link about the skeleton project which was provided by **udacity** in rubric structure.
- After extracting the download project from GitHub, I observed the entire file structure(1.`css/app.css`,2.`img/`,3.`js/app.js`,4.`index.html`,5.`README.md`)

### Some changes in the Code ###

- When I open the project at first there is an empty page with an error in display _allEnemies_.
- Then I created a class for actor and I entered values to it.
- I initialized actor as player variable.
- In order to run the game I initialized the following function for the bug.
    + `update()`
    + `render()`
    + `handleInput()`
- For updating the actor's position `I used update()` function.
- To display actors on canvas I used `render()` function.
- For handling the input given by the player I used `handleInput` function.
    + left arrow: It is used to move the actor to left side until he reaches the final position at left side.
    + Right arrow: It is used to move the actor to right side until he reaches the final position at right side.
    + Up arrow: It is used to move the actor to top side until he reaches the final position at Up side.
    + Down arrow: It is used to move the actor to bottom side until he reaches the final position at Bottom side.
- Everytime when the actor reaches the water layer, the points will be incremented by 50 points.
- `update()` and `render()*` functions are also used for implementing enemy activities.
- I displayed 3 enemies on canvas based on Graphical measurements using an array.
- To display score of game output display I used innerHTML method.
- If the actor touches the bug(i.e. enemy), the actor will be killed, then the score and restart buttons will be displayed and these are implemented using SweetAlert.

## How to play this game?
- Open root file (`index.html`) in any web browser.
- Move the player by using the direction keys on the keyboard.
- If the moves reaches to the water area, the points will be increased by 25. ( Initially the counter is initialized with `0`).
- The player have to reach the water area with out touching any bug on the canvas.
- If he touches the enemy or bug, then he restarted from the his initial position.
