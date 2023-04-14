### Counting the number of characters
Create a program that prompts for an input string and displays output that shows the input string and the number of characters the string contains.

inputs:
- word: a string - It can contains any characters as a string except ""
process:
- countCharacters
output:
- word and numberOfCharacters: a string

testCases:
----------
1. 
input for word: None
expected output: error message "Please enter your a word"
2. 
input for name: Erdogan
expected output: "Hello Erdogan"
3. 
input for name: 1234
expected output: error message "Please enter a valid name"

Process:
========
1. Ask users for name
2. Check the name if it is empty or any number
2.a. If everythings is ok: Go step 3
2.b  If everything is not ok: Go step 1 again with error message
3. Combine the name with 'Hello '
4. Print the greeting name

Refine process:
===============
Prompt "Please enter your name"
Set given name as in the name variable
Check name:
    If it does not works
        error = true
    Else 
        continue
    END IF
    If error
        Display "Please enter a valid name"
        Go back to prompt
Set greetingName = "Hello " + name
Print greetingName

