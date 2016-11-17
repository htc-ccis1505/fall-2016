---
title: "Basic Ruby Class"
published: true
morea_id: ex-basic-class
morea_type: experience
morea_summary: "Let's write a basic class in Ruby!"
morea_sort_order: 1
---

# {{ page.title }}
{{ page.morea_summary }}

## Starter files from GitHub
Use the following link to create your own repository to submit the assignment on GitHub:
[Ruby Lab 5](https://classroom.github.com/assignment-invitations/d7a5597ac5b71534691697d6407b9598)

Click the link to have the assignment created for you, then click the link to go to your personal assignment repository on GitHub.

## Make a Die class
We're going to make a class for a multi-sided [die](https://en.wikipedia.org/wiki/Dice).  

The die should have two properties:

- a number of sides
- the "shown" side (the value that would be read for the roll)

And two behaviors:
- roll - generates the random number for the roll, setting the "shown" side
- get showing -  returns the number on the "shown" side, the number that would be read for the most recent roll.  Note that this should not roll the die, it should just read the roll.

There is an example of a Die class in the reading, but it is just a standard 6-sided die.  You can start with this example, but it is not complete.  This class should allow different numbers of sides.  

Technically a die can't really be 1, 2, or 3 sided - and some numbers of sides are more "fair" than others, but for right now we're going to ignore most of this.  We can have the code that creates the die prevent certain numbers, but for now we'll leave that out of the class itself.  

## Write a test script
Test your object by creating code to:

- Ask the user how many sides their Die should have
- Don't accept numbers less than 4.  Give an error and ask again.
- Create a new instance of the Die class that has that number of sides
- Repeat asking the user if they want to roll the die.  Stop when they say "No".  Make this check case in-sensitive.  It should stop for "NO", "no", or any combination of upper/lowercase letters.
- When they say no (again, case insensitive), ask them if they would like to create a different die.  If they say no, end the program.  If they say yes, repeat these steps.
