# Magic8Ball

A simple command-line Magic 8 Ball game written in Python. This script simulates the classic toy by providing random yes/no responses to user questions.

## Features

* Reads a list of Magic 8 Ball-style responses from a text file
* Allows users to ask yes/no questions interactively
* Randomly selects and displays a response to each question
* Clean exit using the `'quit'` command
* Easy to customize responses via an external file

## How It Works

* The program loads all possible responses from a file named `8ball_responses.txt`, with one response per line
* It then enters a loop, prompting the user to ask a yes/no question
* For each question:

  * A random response is selected using Python's `random.choice()`
  * The response is displayed to the user
  * The loop continues until the user types `'quit'`

## Sample `8ball_responses.txt`

Yes, definitely.
Ask again later.
My sources say no.
Without a doubt.
Cannot predict now.
Very doubtful.

## Sample Interaction

Ask a yes/no question (or type 'quit' to exit): Will I get the job?
My sources say no.

Ask a yes/no question (or type 'quit' to exit): Is today my lucky day?
Without a doubt.

Ask a yes/no question (or type 'quit' to exit): quit
Goodbye!

## Code Overview

**get\_responses\_from\_file(filepath)**
Reads all responses from the specified text file and returns them as a list.

**magic\_8\_ball()**
Handles the main interaction loop:

* Prompts the user for input
* Selects a random response
* Ends when `'quit'` is entered

**main()**
Initializes the game and starts the interaction.

---
