# Bug List

> Make a list of the things that don't work as expected. Keep a list of things that you have fixed and try to document how you solved them.

## 1. Problem: *Letters not updating on screen* 
**Problem:**
User input was not updating the dashed word display correctly.

**Solution:**
Used `split()` and `join()` to manage the guessed word as an array and update it dynamically.First i tested the updated letters in the console, then displayed them on the HTML page.

## 2. Problem: *Repeated letter selection* 
**Problem:**
User could click the same alphabet button multiple times.This also reduced the chances each time the same letter was clicked.

**Solution:**
Used `disable = true` after a button was selected.This is how two problems were solved.This prevented the user from clicking the same button again and stopped chances from decreasing repeatedly for the same letter.

## 3. Problem: *Feedback not visible after correct guess* 
**Problem:**
Next word loaded immediately, so the user could not see the success message.

**Solution:**
Used `setTimeout()` to delay loading the next word by 5 seconds, so the user can see the feedback message.

## 4. Problem: *Hint button clickable at wrong time* 
**Problem:**
User could click the hint button at the wrong time for example after guessing a word incorrectly (When  the lose message is displayed on screen).

**Solution:**
This problem was solved by making hint button disable after an incorrect guess so the user only sees the lose message without interruption.

## 5. Problem: *Repeatition of same random word* 
**Problem:**
Previously used words were appearing again.

**Solution:**
Created a `usedIndexes` array to store generated random indexes.Each time a new word is selected, the index is checked against this array.If it already exists, a new index is generated.This prevents repetition and ensures unique words.

## 6. Problem: *Game not resetting properly* 
**Problem:**
Old messages remained when next word loaded.

**Solution:**
This problem was solved by clearing the previous messages before loading next word.

## 7. Problem: *Keyboard input issues* 
**Problem:**
   - Multiple characters accepted.
   - Special keys also accepted .

**Solution:**
Restricted keyboard input to a single alphabet character from a to z.This means that special keys and other characters are ignored and an alert message is shown when invalid input is entered. 

## 7. Problem: *Not loading the next word after refreshing within 5 seconds delay time* 
**Problem:**
The game stucks when page is refreshed within 5 seconds delay time(Time for loading next random word).

**Solution:**
Declaring and assigning variable `problem` true so that wordsDisplay function is called from loadGame function after refresh.This removes the bug.

 