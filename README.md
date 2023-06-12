Classic hangman game made in React with useState to track user input (guesses) and word to guess. Logic connected through useEffect where keypresses would be handled to update state

Design Process
-Need to track user input, new word to guess, and compare the two
-useEffect to handle each keypress and invoke a callback function to store the pressed letter
-filter the array of guessed letters to get new array for incorrect keypresses by comparing it with the stored wordToGuess
-loss/win conditions: loss if # of guessed letters is greater than length of wordToGuess. win if wordToGuess letters exist inside array of guessed letters
-hangman drawing is based on # of incorrect letters
-pass guessedLetters and wordToGuess to reveal which correct letters have been guessed
-pass guessedLetters and wordToGuess to Keyboard component to highlight letters being guessed
