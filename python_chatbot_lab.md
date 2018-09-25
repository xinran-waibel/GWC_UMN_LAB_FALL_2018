# Python Chatbot Lab
![chatbot_image](https://regmedia.co.uk/2017/09/21/chatbot.jpg?x=442&y=293&crop=1)

## Introduction
Hello there! Welcome to the Python Chatbot Lab! In this lab, you will start by learning/reviewing Python basics. Then you will build a working chatbot in Python that you can interact with via Command Line Interface (CLI)! In each section, there will be **Examples** and **Tasks**:
- Example: instructions and source code for you to learn and try yourself
- Task: coding problems similar to its corresponding Example for your to solve

### Q&A: What is Command Line Interface
A command-line interface (CLI) is a way of interacting with a computer program where the user (YOU) gives commands to the program in the form of successive lines of text (aka command lines).

## Open a Python CLI
- Go to Start
- Search for Python
- Click and open IDLE and you will see a window like below:

···![idle_image](https://github.com/xinranduan/GWC_UMN_FALL_2018/blob/master/images/python_idle.png)

- Now you are able to issue commands by typing Python code into CLI

### Q&A: What is IDLE
IDLE is an powerful development environment for Python that includes both Python CLI and Python file (.py) editor, which we will learn and use in this lab. Please note that you can still write Python code and issue Python commands without IDLE, as long as Python is installed.

## Python Basics
### [Example 1]
Let's first write a Python statement to output/display Hello World using `print()` function:
```python
print('Hello World')
```

Copy and paste the statement above to your CLI and press `Enter` button to issue the command.
### [Task 1]
Write a line of Python code to display your favorite quote using `print()` function
#### Q&A: What does `print()` do?
`print()` function prints the specified message to the screen

#### Q&A: What is a function?
A function is a block of code which is used to utilize code in more than one place and only runs when it is called. You can pass data, known as parameters, into a function. A function can return data as a result. `print()` is a build-in function in Python, which means its code is written by Python's developers for our convince. As Python users, we can create our own functions too using `def`.

### [Example 2]
Let's try display variables. I want to display a introduction of myself in two lines on the screen:
··· My name is Xinran
··· Xinran is pronounced as SHEEN-ran

Store my name and my name's pronunciation as variables and then use the variable in my `print()` statements:
```python
my_name='Xinran'
my_name_pron='SHEEN-ran'
print('My name is', my_name)
print(my_name, 'is pronounced as', my_name_pron)
```
#### Q&A: What is a variable?
A variable is an object in Python that has a name and a value, and we can refer to a variable by its name. For example, in the code above, my_name is a variable whose name is `my_name` and has value `'Xinran'` assigned to it.

### [Task 2]
Print a short introduction of yourself in following format using variables, for example:
- My favorite color is xxx
- The opposite color of xxx is yyy

(Please store xxx and yyy as variables and then use `print` to display your introduction lines.)

### [Example 3] 
Instead of using commands/statements line by line using Python CLI, let's put multiple commands together in a Python file to be more efficient:
* In CLI, click `File` -> `New File`
* Now you should be in a Python editor window that shows an empty Python file

Sometimes I have a hard time deciding what to eat for lunch: Healthy Salad, Burger and Fries, or Dumplings, so I write a program to randomly decide for me:
``` python
import random

lunch_options = ['Healthy Salad', 'Burger and Fries', 'Dumplings']
random_lunch = random.choice(lunch_options)
print('My lunch will be', random_lunch)
```

In the code above:
- `import random` allows us to use functions defined in `random` library so we don't need to write ourself
- `lunch_options` is variable and its value is a `list` of food options
- `random.choice` is the a function called `choice` in `random` library that can randomly pick an element from a `list` (p.s. each element has roughly the same chance to be selected.)

Copy and paste the code to your Python editor and save your Python file. Click `Run` -> `Run Module` to run/execute the Python file and you will see the output in the pop-up Python CLI. So, what will my lunch be?

### [Task 3]
Suppose we have only one pizza slice left in the pizza box, but all TAs are still hungry so they all want want it! Please write a Python program to help us decide who will get the last slice of pizza.

### [Example 4]
Here is a Python program to help me find out all natural numbers smaller than 20 that are multiples of 3, 7:
```python
number = 1
while (number < 20):
    if (number % 3 == 0):
        print (str(number), 'is a multiple of 3')
    elif (number % 7 == 0):
        print (str(number), 'is a multiple of 7')
    number += 1
```

In the code above:
* By using `while(condition)`, all the statments in the `while` block will be executed repeatedly as long as `condition` is evaluated to `True`
* `number += 1` is equalvalent to `number = number + 1`, which increments the value of variable `number` by one

### [Task 4]
Write a Python program to compute the sum of all even numbers smaller than 11

## Build a Chatbot

### Basic functionalities of a chatbot:
A chatbot gives different responses (output of chatbot) depending on what messages it received (input of chatbot). For example, if the input is some form of greetings, the output should be a greeting too. If the input is some kind of small talks (like 'How are you?'), the output can be 'OK', 'Good' or whatever is appropriate. Chatbot should be able to keep talking to the user, in other words keep asking for user input.

Also consider following cases:
- What if the chatbot does not 'understand' the user input?
- When should chatbot stop talking?

**Hint**
- Chatbot should have a 'knowledge bank'
- Think about what you have learned in `Python Baics` section
- You can use `input()` to ask for user input and store the user input in a variable called `user_input` to be used later. When we pass '>> ' as prompt argument to `input()`, '>> ' will display in front of user input area.
```python
user_input = input('>> ')
```
