# Introduction to Shell Scripting and User Input
## Shell Scripting Syntax Elements
### (1). Variables: Bash allows you to define and work with variables. Variables can store data of various types such as numbers, strings, and arrays. You can assign values to variables using the = operator, and access their values using the variable name preceded by a $ sign. 
#### Example: Assigning value to a variable:
$ name="John"
#### Example: Retrieving value from a variable:
$ echo $name
![Screenshot from 2023-10-02 16-29-18](https://github.com/PromiseNwachukwu/Shell-Scripting-Hands-on-Project/assets/109115304/a3fe1cab-1a25-4d52-9552-1aed5bd6dda1)

### (2). Control Flow:  Bash provides control flow statements like if-else, for loops, while loops, and case statements to control the flow of execution in your scripts. These statements allow you to make decisions, iterate over lists, and execute different commands based on conditions. 
#### Example: Using if-else to execute script based on a conditions
![Screenshot from 2023-10-02 20-18-29](https://github.com/PromiseNwachukwu/Jenkins-CICD-practice/assets/109115304/5b822630-ddb6-4500-a243-4dceea88c5b9)

#### Iterating through a list using a for loop
![Screenshot from 2023-10-02 21-06-34](https://github.com/PromiseNwachukwu/Jenkins-CICD-practice/assets/109115304/7828b76d-d875-4d9f-9e4d-255380f5d676)

### 3. Command Substitution: Command substitution allows you to capture the output of a command and use it as a value within your script. You can use the backtick or the $()syntax for command substitution. 
#### Example: Using backtick for command substitution
$ current_date=`date +%Y-%m-%d`
#### Example: Using $() syntax for command substitution
$ current_date=$(date +%Y-%m-%d)
![Screenshot from 2023-10-02 21-49-46](https://github.com/PromiseNwachukwu/Shell-Scripting-Hands-on-Project/assets/109115304/47e64f9b-a723-4ee7-a5ce-f7216128fdfc)

### (4). Input and Output: Bash provides various ways to handle input and output. You can use the read command to accept user input, and output text to the console using the echo command. Additionally, you can redirect input and output using operators like > (output to a file), < (input from a file), and | (pipe the output of one command as input to another). 
#### Example: Accept user input
$ echo "Enter your name:"
$ read name
#### Example: Output text to the terminal
$ echo "Hello World"
#### Example: Out the result of a command into a file
$ echo "hello world" > index.txt
![Screenshot from 2023-10-02 22-22-36](https://github.com/PromiseNwachukwu/Shell-Scripting-Hands-on-Project/assets/109115304/c8caa62a-4eb7-49fa-be35-1fcf90e9be0a)

### (5),Functions: Bash allows you to define and use functions to group related commands together. Functions provide a way to modularize your code and make it more reusable. You can define functions using the function keyword or simply by declaring the function name followed by parentheses. 
![Screenshot from 2023-10-02 23-39-13](https://github.com/PromiseNwachukwu/Shell-Scripting-Hands-on-Project/assets/109115304/0278d3c7-e1d5-47c8-8e36-c900234c036b)


## Writing our First Shell Script
#### step 1: On your terminal, open a folder called shell-scripting using the command mkdir shell-scripting. This will hold all the script we will write in this lesson.
#### step 2: create a file called user-input.sh using the command touch user-input.sh
#### step 3: Inside the file copy and paste the block of code below:
$ #!/bin/bash

$ # Prompt the user for their name
$ echo "Enter your name:"
$ read name

$ # Display a greeting with the entered name
$ echo "Hello, $name! Nice to meet you."

#### A liitle bit about the code block. The script prompts for your name. When you type your name, it displays the text hello ! Nice to meet you. Also #!/bin/bash helps you specify the type of bash interpreter to be used to execute the script.
#### step 4: save your file
#### step 5: Run the command sudo chmod +x user-input.sh this makes the file executable
#### step 6: Run the script using the command ./user-input.sh
![Screenshot from 2023-10-02 23-43-28](https://github.com/PromiseNwachukwu/Shell-Scripting-Hands-on-Project/assets/109115304/c7f79ad4-9923-45ec-bc8b-70cd09731fb2)

## Directory Manipulation and Navigation
#### Writing sample shell script. 
![Screenshot from 2023-10-02 23-58-01](https://github.com/PromiseNwachukwu/Shell-Scripting-Hands-on-Project/assets/109115304/b035a551-fe27-4860-ab9c-cd8729aeac03)

#### Directory Manipulation and Navigation
##### Proceed by following the steps bellow:
$ step 1: open a file named navigating-linux-filesystem.sh
$ step 2: paste the code block below into your file.
$ step 3: Run the command sudo chmod +x navigating-linux-filesystem.sh to set execute permission on the file
$ step 4: Run your script using this command ./navigating-linux-filesystem.sh
![Screenshot from 2023-10-03 00-24-27](https://github.com/PromiseNwachukwu/Shell-Scripting-Hands-on-Project/assets/109115304/fb67d259-0605-423b-8e96-0fc04052cbea)

## File Operations and Sorting
#### Writing a simple shell script that focuses on File Operations and Sorting.
#### This script creates three files (file1.txt, file2.txt, and file3.txt), displays the files in their current order, sorts them alphabetically, saves the sorted files in sorted_files.txt, displays the sorted files, removes the original files, renames the sorted file to sorted_files_sorted_alphabetically.txt, and finally displays the contents of the final sorted file.
![Screenshot from 2023-10-03 00-37-18](https://github.com/PromiseNwachukwu/Shell-Scripting-Hands-on-Project/assets/109115304/323d5687-0f47-4df7-9c58-2b61c5d372a5)

#### Excercise on File Operations and Sorting
$ step 1: Open your terminal and create a file called sorting.sh using the command touch sorting.sh
$ step 2: Copy and paste the code block below into the file
$ step 3: Set execute permission on sorting.sh using this command sudo chmod +x sorting.sh
$ step 4: Run your script using the command ./sorting.sh
![Screenshot from 2023-10-03 00-43-20](https://github.com/PromiseNwachukwu/Shell-Scripting-Hands-on-Project/assets/109115304/9fda6e13-c311-41f7-b8dc-f06a855af965)

## Working with Numbers and Calculations
$ step 1: On your terminal create a file called calculations.sh using the command touch calculations.sh
$ step 2: Copy and paste the code block below:
$ Step 3: Set execute permission on calculations.sh using the command: sudo chmod +x calculations.sh
$ step 4: Run your script using this command: ./calculations.sh
![Screenshot from 2023-10-03 00-53-37](https://github.com/PromiseNwachukwu/Shell-Scripting-Hands-on-Project/assets/109115304/5599d7f2-c139-4d82-a699-e47889a033cb)
