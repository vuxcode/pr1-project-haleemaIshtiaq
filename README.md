[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/F4JWjZ9e)
# Project Instructions
Follow the instructions here: https://vuxcode.netlify.app/new/pr1/lessons/major-project-brief/

REMEMBER TO "COMMIT" YOUR CHANGES REGULARLY TO SHOW HOW YOU HAVE BUILT THIS PROJECT! 

The final program is not the goal! The aim of the project is to show how you have developed your program, the steps you have taken and the problems you have solved!

# Project Notes

> You can use this section of the file to keep notes about your project as you work on it.

# Project Summary

> Before the final submission date you should include a "PROJECT SUMMARY" in this section here. 

"Hangman Word Guessing Game" is an interactive game developed using HTML, JavaScript and Canvas.The project was created to improve    understanding of JavaScript concepts, event handling and Canvas drawing.

The game allows users to select between two modes: Time Based mode and Without Time mode.In the Time Based mode, the player must guess the hidden word within a limited time of two minutes while the Without Time mode allows the user to play without any time restriction.
 
Users can guess letters either by clicking the alphabet buttons on the screen or by using the keyboard.The alphabet buttons from A to Z were generated dynamically using JavaScript and ASCII values.keyboard input and button clicks were synchronized so that both methods work together.

The project includes five categories( animals,countries,technology,food and nature).Radio buttons were used for category selection so that only one category can be selected at a time.Separate word arrays and corresponding hint arrays were created for each category.

Canvas was used to draw the Hangman drawing step by step according to the user's wrong guesses.Additional features such as hints,remaining chances,number of  guessed words, win and lose messages,button disabling and keyboard validation were also implemented.A Quit button was also added to allow the users to leave the game at any time.A Countdown timer is also displayed on the screen in Time Based mode.

A refresh feature was developed using localStorage.Functions such as saveGame(),loadGame()and recolouringKeypad() were created to restore game progress, keypad button states and other game data after a page refresh.This feature has been added after a user selects a category.

#### *Development Experience*:

While developing this project many JavaScript concepts were learned and practiced including functions, loops, arrays, event handling, querySelector, localStorage, attributes and Canvas drawing.

One of the biggest learning experiences was creating the Hangman drawing using Canvas.This helped in understanding how canvas coordinates and drawing functions work.Another important learning experience was creating buttons dynamically and connecting keyboard input with button clicks using event listeners and custom attributes.Implementing the refresh feature to restore game data was also challenging but educational.

Several bugs occurred during project development especially related to repeated key presses, invalid keyboard input, refresh issues and restoring button colours.Forexample the game became stuck when the page was refreshed during the five seconds delay before loading the next word.These problems were solved through debugging, testing and improving the program logic.Overall the project helped improve problem solving skills and understanding of JavaScript development.


#### *Possible Improvements*:

- Add difficulty levels such as easy, medium and hard.
- Add sound effects and animations.
- Store player data in database.

#### *Budget Conclusion*:

The project didnot require any financial budget because all tools used were free.The main investment was the time spent on developing the project.

The estimated development time for the project was 30 hours but the actual development time became approximately 45 hours.This is because additional time was spent implementing the refresh feature to restore game data after page refresh, which was not included in the planning.

Although the project exceeded the planned time budget, the extra development time helped improve problem solving skills and understanding of JavaScript concepts.


# User Guide

> Write a clear user guide for how someone should use your program.