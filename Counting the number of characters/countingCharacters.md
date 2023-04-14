### Counting the number of characters
Create a program that prompts for an input string and displays output that shows the input string and the number of characters the string contains.

inputs:
- word: a string - It can contains any characters as a string except ""
- numberOfCharacters - Integer
process:
- divideCharactersIntoLetters
- countCharacters
- displayResult 
output:
- word and numberOfCharacters: a string

testCases:
----------
1. 
input for word: None
expected output: error message "Please enter something"
2. 
input for word: Erdogan
expected output: "Erdogan 7"
3. 
input for word: 1234
expected output: "1234 4"

4. input for name: <script> 
expected output: error message "Please enter a valid name"

5. input for name: },{, [], :, ;, & - They should be checked separately for all
expected output: error message "Please enter a valid name"

6. input for name: ADD, DELETE, SELECT, UPDATE, WHERE - They should be checked separately for all
expected output: error message "Please enter a valid name

Process:
========
1. Ask users for a word
2. Check the name if it is empty or a malicious attack
2.a. If everythings is ok: Go step 3
2.b  If everything is not ok: Go step 1 again with error message
4. Divide the word into letters one by one
3. Count the characters
4. Print the word and number of characters

Refine process:
===============
Initialize numberOfCharacters to 0
Prompt "Please enter a word"
Set given name as in the word variable
Check word:
    If it does not works
        error = true
    Else 
        continue
    END IF
    If error
        Display "Please enter a valid name"
        Go back to prompt
Loop for word
    Increase numberOfCharacters with 1
Revert numberOfCharacters to String
Print word + " " + numberOfCharacters



