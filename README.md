---
module: mark-induction

level: 2

methods:
  - team
  - pair
  - solo

tags:
  - wip
---

# String functions

<a rel="license" href="http://creativecommons.org/licenses/by-nc-nd/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-nd/4.0/88x31.png" /></a>

> This is part of Academy's [technical curriculum for **The Mark**](https://github.com/WeAreAcademy/curriculum-mark). All parts of that curriculum, including this project, are licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-nd/4.0/">Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License</a>.

## Learning Outcomes

- Follow TDD principles: write tests and then the code to pass them
- Work with a partner across both of your machines

## Prerequisites:
- Install `pytest`

## Key themes

This exercise is about how to collaborate across machines with GitHub so you will need to work with your partner. 

At every step, try to predict the response of git status before checking it.

Make sure to commit your code regularly and push to remote. Continue switching between the two machines (and so you will need to keep GitHub up to date) through the exercises.

We will be practicing TDD throughout these exercises - write your tests first and then write the code required to pass them. We will be completing challenges working with strings to practice this. After, please continue using similar methods to approach other katas.

## Exercise 0: Set up and initialise your local repository (Machine A)

> 🎯 **Success criterion:** You are able to create the directory using the command line and initialise a local repository.

- Create a new directory within `Academy`
- Initialise a new git repository within it
- Create a sub-directory `src` (short for "source")

## Exercise 1: Write the first tests for `capitaliseString` and push to GitHub (Machine A)

> 🎯 **Success criterion:** You have written your first tests and pushed them to a remote repository.

- Create a python file within it `main.py`
- Make an initial commit
- In `main.py`, define a function `capitaliseString` which takes a single string parameter. To begin with, make it return that same string
- Create a python file `main_test.py` which we will use to test the program
- Write a test for the function `capitaliseString`: check that it returns a given word in capitals
- Commit your first test
- Write three more tests for `capitaliseString` giving it other words
- Run your tests using `pytest` - you will see that they fail
- Commit your work and continue to commit regularly as we go along
- Create a new repository on GitHub
- Push your work to the remote repository
- Send the url of the repository to your partner

## Exercise 2: Clone the repo onto a different machine and make `capitliseString` pass the tests (Machine B)

> 🎯 **Success criterion:** You have cloned the repository onto a second machine, written the function body to pass the tests and pushed back to remote.

- Clone the repository onto the other member of the pair's machine.
- Investigate the files - notice how the setup of the repository is preserved , i.e. both `main.py` and `main_test.py` are within the `src` sub-directory just like on the original machine.
- Investigate the git log - see that all of the commits on your partner's machine are also present and viewable here.
- Run the tests with `pytest` - they will fail again
- Write the function body of `capitaliseString` so that it passes the initial tests.
- Check that it passes the tests.
- Push to remote - you should do this regularly so that it is always available online (for your own benefit if your laptop were to have a problem and for your team's benefit so they can see the most recent version).

## Exercise 3: Pull the latest changes onto the original machine and write some more tests (Machine A)

> 🎯 **Success criterion:** An expanded test suite.

- Switch back to Machine A.
- Pull the latest changes in.
- Run the tests again to prove that they are passing.
- Expand the test suite - add tests to check `captiliseString` works with a multi-word phrase.
- What happens if the input includes numbers or punctuation in the string? Add tests for this.
- Run your tests: if they fail then improve your function to resolve this.
- Commit and push to remote - keep doing this regularly.

From here onwards, keep committing and pushing. Swap between machines regularly to take turns.

## Exercise 4: Lower case strings

> 🎯 **Success criterion:** A function and relevant tests for it to change a string into lowercase.

Now let's make a new function `decapitaliseString` which does the opposite of `capitaliseString`: it should turn any capital letters into lower case.

- Similarly to before, start by defining the function and making it return something abritrary such as its input. It should take a string as its only parameter.
- Write a thorough test suite for this function - think about cases such as number, punctuation, words with spaces, and anything else which may come up.
- Write the function itself and ensure it passes all your tests.
- Write additional tests if you thought of any in the meantime.

## Exercise 5: Capitalise the first letter of every word in a string

> 🎯 **Success criterion:** A function and relevant tests for it to capitalise the first letter of every word in a string. 

Make a new function to capitalise the first letter of every word in a string (and make all the other letters in that string) and write the revelant tests for it. 

If you use helper functions to achieve this then you should also write tests for them.

Example: if we input `hello world` then we would expect an output of `Hello World`.

### Extension: Title case

In title case, most words are capitalised except for "minor words" such as `the` or `a`. Minor words are only capitlised if they appear are the first or last words in the title (or in our case string). More info can be found [here](https://en.wikipedia.org/wiki/Title_case).

Make a function to turn strings into title case. Find a list of minor words online or list some of your own. Test the function with common book or film titles. 

## Exercise 6: Reverse a string

> 🎯 **Success criterion:** A function and relevant tests for it to reverse a string.

Make a new function which reverses strings. Continue using TDD and so write the tests for it first!

## Extension:

Continue practicing TDD to solve challenges and collaborating via GitHub. We recommend looking at katas available on CodeWar for these challenges. 
