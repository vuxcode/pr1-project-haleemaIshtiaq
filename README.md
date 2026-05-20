[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/F4JWjZ9e)
# Project Instructions
Follow the instructions here: https://vuxcode.netlify.app/new/pr1/lessons/major-project-brief/

REMEMBER TO "COMMIT" YOUR CHANGES REGULARLY TO SHOW HOW YOU HAVE BUILT THIS PROJECT! 

The final program is not the goal! The aim of the project is to show how you have developed your program, the steps you have taken and the problems you have solved!

# Project Notes

> You can use this section of the file to keep notes about your project as you work on it.

Worked on the basic game layout using HTML. Created two game mode buttons: "Time Based Game" and "Without Time".

Worked on displaying blank spaces for the random word. Taken an array of only three words to test whether the functionality worked correctly. Successfully implemented this using join(), split() and repeat() functions. Generated a random number to select a random word from the array. Fixed a bug where the same random word was repeatedly selected by using an array called (usedIndexes). This bug was easier to solve after tracking previously used random indexes. After testing, confirmed that all features worked properly, the word array size was increased from three to ten words.

Created an empty `div` in HTML to store dynamically generated alphabet buttons. Experimented with dynamic button generation using ASCII values in JavaScript instead of using a static HTML approach of manually creating 26 alphabet buttons.Learned about DOM (Document Object Model) manipulation which allows JavaScript to create, modify and manage HTML elements dynamically.

Created a Hint button and worked on the hint array. Worked on words guessed  and remaining chances counters. After completing these features, still thinking about how to draw Hangman.Thought about using images for Hangman.

Attended the last lecture with the teacher and learned about Canvas, decided to use Canvas for drawing Hangman instead of images. Learned about cordinates (x and y) in Canvas and also experimented with the free tool Desmos to understand coordinates visually. Learned that the y-coordinate system in Canvas is different from the actual mathematical coordinate system because in Canvas the y-value increases downward.

Calculated Desmos y-coordinate using:

`Desmos y = 300-Canvas y `

where 300 pixels is the Canvas height set in the program.

Today attended the workshop and liked the teacher's suggestion of using keyboard input along with the on screen buttons. Got help from the teacher to implement keyboard input. It was easier. Completed this in the same workshop but still thinking about synchronizing the game keypad with the keyboard input.

Succeeded in synchronizing keyboard input with game keypad buttons after learning about custom HTML attributes using `setAttribute()` and `querySelector()`.

Many friends tried the game and suggested improving it by introducing categories because it was difficult to guess the hidden words without any context. Got the idea of adding categories such as animals, food, nature, countries, technology to make the game easier and more interseting.

After completing the project according to the planning, wanted to add one more feature because extra development time was still available.
Introduced a refresh feature using `localStorage()` to restore game data after page refresh.




# Project Summary

> Before the final submission date you should include a "PROJECT SUMMARY" in this section here. 

` "Hangman Word Guessing Game" ` is an interactive game developed using HTML, JavaScript and Canvas. The project was created to improve    understanding of JavaScript concepts, event handling and Canvas drawing.

The game allows users to select between two modes: `Time Based mode` and `Without Time mode`. In the Time Based mode, the player must guess the hidden word within a limited time of two minutes while the Without Time mode allows the user to play without any time restriction.
 
Users can guess letters either by clicking the alphabet buttons on the screen or by using the keyboard. The alphabet buttons from A to Z were generated dynamically using JavaScript and ASCII values. Keyboard input and button clicks were synchronized so that both methods work together.

The project includes five categories( Animals, Countries, Technology, Food and Nature). Radio buttons were used for category selection so that only one category can be selected at a time. Separate word arrays and corresponding hint arrays were created for each category.

Canvas was used to draw the Hangman drawing step by step according to the user's wrong guesses. Additional features such as hints, remaining chances, number of  guessed words, win and lose messages, button disabling and keyboard validation were also implemented. A Quit button was also added to allow the users to leave the game at any time. A Countdown timer is also displayed on the screen in Time Based mode.

A refresh feature was developed using localStorage. Functions such as saveGame(), loadGame() and recolouringKeypad() were created to restore game progress , keypad button states and other game data after a page refresh. This feature has been added after a user selects a category.

#### *Development Experience*:

While developing this project many JavaScript concepts were learned and practiced including functions, loops, arrays, event handling, querySelector, localStorage, attributes and Canvas drawing.

One of the biggest learning experiences was creating the Hangman drawing using Canvas. This helped in understanding how canvas coordinates and drawing functions work. Another important learning experience was creating buttons dynamically and connecting keyboard input with button clicks using event listeners and custom attributes. Implementing the refresh feature to restore game data was also challenging but educational.

Several bugs occurred during project development especially related to repeated key presses, invalid keyboard input, refresh issues and restoring button colours. Forexample the game became stuck when the page was refreshed during the five seconds delay before loading the next word. These problems were solved through debugging, testing and improving the program logic. Overall the project helped improve problem solving skills and understanding of JavaScript development.


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

1. Open a game in a web browser.

2. User can see the welcome message and two buttons.

      - Time based game (Time limit 2 minutes)
      - Without Time (No time limit)

    Choose a game mode by clicking one of the above buttons.    

3. Click one of the five category buttons.

      - Countries
      - Animals
      - Technology
      - Food
      - Nature

4. After selecting the category, click the `Start Game` button below the categories.

5. After clicking the `Start Game` button , the game starts and the user can see the following:
    
    * Left side
      
      - Countdown timer 2:00 ( Only for Time Based mode )
      - words guessed: 0/5 ( This shows the number of correctly guessed words )
      - chances left: 6/6   ( This shows the number of chances left)

    * Right side 

      - Hangman drawing (Initially only stand is displayed. The hangman is drawn step by step after wrong guesses) 

    * Bottom left

      - `Quit` button to leave the game at any time.  

    * Center

      - Hidden word represented using blank spaces (-----).
      - `Hint` button for displaying hint.
      - Keypad ( Alphabet buttons from A to Z )

6. Start guessing the hidden word by:

      - Clicking the alphabet buttons on the screen or
      - Pressing keyboard letters from A to Z

    **OBS:**  The game only accepts alphabet letters from A to Z. Alert messages are displayed for invalid or repeated keyboard inputs. The game automatically disables already used buttons so the chances do not decrease for the same wrong letter again.

7. Correct guesses reveal letters in the hidden word.

8. Wrong guesses draw parts of the Hangman and reduce the remaining chances.

9. Click the `Hint` button if you need help related to the hidden word.

10. On guessing the hidden word correctly , the next word is automatically displayed and the "words guessed " counter on the screen is updated.

11. The winning criteria is to guess five words correctly consecutively.

12. The game ends if all six chances are lost before guessing the hidden word and the next word is not displayed.

13. In Time Based mode, the game also ends if the two minute countdown timer reaches zero.This means the user must guess all five words correctly consecutively witin two minutes.

13. Winning or losing messages are displayed on the screen.

14. `Restart` and `Exit` buttons are dispayed after the game ends.

15. Use the `Quit` button to leave the game at any time.

16. The refresh feature restores the game progress after a page refresh using local storage.
       

