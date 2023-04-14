### Hello
Create a program that prompts for your name and prints a greeting using your name.

inputs:
- name: a string
process:
- printName
output:
- greetingName: a string

testCases:
----------
1. 
input for name: None
expected output: error message "Please enter your name"
2. 
input for name: Erdogan
expected output: "Hello Erdogan"
3. 
input for name: 1234
expected output: error message "Please enter a valid name"

4. 
input for name: Anna Maria
expected output: Hello Anna Maria"

5. 
input for name: Smith 5
expected output: Hello Smith 5"

6. input for name: <script> 
expected output: error message "Please enter a valid name"

6. input for name: },{, [], :, ;, & - They should be checked separately for all
expected output: error message "Please enter a valid name"

Process:
========
1. Ask users for name
2. Check the name if it is empty, any number or a malicious attack like SQL injection or Javascript
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

