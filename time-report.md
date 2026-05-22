# Time Report

<!-- Write about what you have done and how long you have worked on each part of the project.

For example: -->

## 2022-03-24 18:00 Worked for 1 hour.

 - *Planned the game design.*

      -  listed the main features.
      -  Designed a  basic flowchart for the game flow.
      -  Planned how the Hangman Game interface should looks.
  
## 2022-03-25 10:00 Worked for 1 hour.

 - *Created the first page of the game.*
      
      - Added the main heading and welcome message.
      - Added Time Based and Without Time game mode buttons.

## 2022-03-26 10:00 Worked for 1.5 hour.
 - *Created the second page of the game.*
      
      - Connected buttons using JavaScript event listeners.
      - Created separate functions for Time Based and Without Time modes (buttons).
      - Updated the welcome message when a mode is selected.
      - Added a Hint button.

## 2022-03-27 18:00 Worked for 3 hours.
 - *Worked on displaying the keypad.*
      - Created a `showKeypad` function which includes:
          - Dynamic generation of A-Z buttons using JavaScript.
          - Conversion of ASCII values into letters from A to Z.
          - Displaying of generated buttons on the page using `appendChild()`.
          - Styling of buttons (color, font size, padding and margin).
          - Line breaks to arrange buttons in multiple rows.
       
## 2022-03-30 15:43 Worked for 3 hours.
 - *Worked on random word display.*
      - Created a  `wordsDisplay` function which includes:
          - An Array of words (Initially containing three words).
          - Use of `Math.random()` to select a random word.
          - Displaying of blank dashes based on the length of the selected word.
 - *Tested both game modes and fixed basic display issues.*
 - *Made a first commit after completing initial development(24-30 March)*.

## 2022-04-08 10:00 Worked for 5 hours.
 - *Worked on word display, input handling and game logic improvements.*
      - Created a separate `wordChecking` function to separate the letter checking logic from `wordsDisplay`.
      - Used `split()` and `join()` to manage the guessed word as an array and update it dynamically.
      - Implemented logic to display user-entered characters in the correct positions(tested via console).
      - Replaced `prompt()` input by integrating keypad button input with the `wordChecking` function.
      - Created a `disableButtons` function to disable alphabet buttons after selection to prevent repeated input.
      - Improved win and lose messages and displayed them on the screen.

## 2022-04-09 10:45 Worked for 3 hours.   
 - *worked on hint system .*
      - Created a showHint function.
      - Created an array to provide hints for each word.
      - Developed logic to display the correct hint based on the selected word.
 - *Added hover effects on keypad buttons and added pointer cursor to buttons.*
 - *Created a `div` to display the final game result (win or lose message).* 
 - *Added a `div` to show remaining chances on the screen dynamically.*     

## 2022-04-16 09:00 Worked for 3 hours.    
 - *More worked on hint system.*
      - Created a separate`div` with id `hintText` to show hints clearly on screen.
      - Added logic to hide the hint button after use.
      - Made Hint button disabled if user guess the word wrong and not used the hint.
 - *Improved game flow.*
      - Loads the next word after a correct guess.
      - clears previous messages and hint before showing the next word.
      - Prevents repitition of choosing the same random word with help of index tracking.
 - *Implemented win condition logic.*
      - Display the final message if user guess 5 consecutive words correctly.
      - Used `setTimeout()` to delay 5 seconds in loading the next word so user can see the feedback.
      - Stops the game and disable the buttons when game ends.
 - *Implemented word tracking logic and created a div to display number of correctly guessed words on screen.*   
 - *Added `enableButtons` function to enable keypad buttons for next loaded word.*     

## 2022-04-17 02:00 Worked for 3 hours.     
 - *Implemented a 2-minute countdown timer for Time Based mode.*
      - Created a startCountDown function.
      - Created a `div` to display the counter on screen.
      - Stopped the timer using `clearInterval()` function when time is over and displayed message of time over on screen.

## 2022-04-20 01:00 Worked for 1 hour.      
 - *Created restart and exit buttons.*
      - showRestart function is added to hide all other game elements and display restart and exit buttons.
      - Added event listeners for both buttons.
      - Exit button displays a thankyou message.
      - Restart button reloads the game.

## 2022-04-22 02:00 Worked for 1 hour.  
 - *Created a canvas element and created a function `drawHangman`.*

## 2022-04-23 09:00 Worked for 4 hours.  
 - *Completed hangman drawing using canvas in the drawHangman function.*
 - *Integrated drawing with game logic and finalized the hangman functionality.*   

## 2022-04-28 09:00 Worked for 4 hours.  
 - *Worked on keyboard support.*
      - Added keyboard input so users can eneter letters directly through keyboard.
      - Synchronized keyboard input with keypad buttons on screen.
      - Implemented validation to allow only single aplphabet characters.
      - Added an alert message for already pressed keys.
      
 - *Worked on layout and readability.*
      - Increased font size for better word display.
      - positioned the hangman canvas at the top right. 
      - Enhanced the hangman drawing by increasing line thickness and adding rounded line ends and smoother corners.  

## 2022-04-30 02:00 Worked for 3 hours.    
 - *Implemented category selection feature.*
      - Created radio buttons for five categories.
      - Defined separate word arrays for each category.
      - Integrated selected category with the game logic.
      - Displayed the selected category name on the screen.   

## 2022-05-03 09:15 Worked for 1 hour.  
 - *Added hint support for categories.*
      - Created separate hint arrays for each category.   
      - Displayed hints dynamically based on the selected category. 

## 2022-05-04 to 2022-05-11 09:15 Worked for approx 6 to 8 hours.   
 - *Added refresh feature.*   
      - Created saveGame() function for saving game data.
      - Created loadGame() function for restoring saved values.
      - Created recolouringKeypad() function for restoring keypad buttons colours and states after refresh.
      - Updated other functions to support the refresh feature.
      - Fixed the bugs related to page refresh.
                              





     
