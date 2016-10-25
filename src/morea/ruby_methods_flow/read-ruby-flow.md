---
title: "Ruby: Conditional Statements & Loops"
published: true
morea_id: read-ruby-flow
morea_summary: "Chapter 7 - Flow."
morea_type: reading
morea_sort_order: 2
morea_labels:
 - ruby
 - textbook
---

# {{ page.title }}
Read through Chapter 7 in the printed textbook, or Chapter 6 in the online [Learn to Program](https://pine.fm/LearnToProgram/chap_06.html), which covers how to work with strings of text in Ruby.

As you read through the text, make sure you are sitting at your computer and trying the commands in interactive ruby from the shell.  

## Note on Equality vs Assignment
Note that in Ruby a single = will do a variable assignment and double == will test for equality. Confusing the two is a __very__ common error.

## Indentation
While it is not syntactically required that you indent your code inside of branching and looping code, you may loose points for this as it makes your code less readable and more likely to contain errors.  

## Review Questions

- How would you determine if a number was less than zero?
- How would you determine if a variable was equal to 42?
- How would you determine if a letter was not a vowel?
- Write code to ask for a number then say whether is it greater than, equal to, or less than zero.
- How would you write a loop to say hello 3 times?
- What does `break` do and why might you use it?
- Why is `while 'Spike' > 'Angel'` the same thing as saying `while true`?  (Note this is a Ruby question where the answer is absolute, not a Buffy question where opinions may differ.)
- What is that `elsif` word used for?
- What is the DRY rule?  (Someone might mention this someday in an interview...)
- What does `true || false` evaluate to?
- What does `true && false` evaluate to?

## Try It!

- Write a __DRY__ script to print the lyrics to 99 Bottles of Beer on the Wall.
- Write the *Deaf Grandma* program described in the text.
    1. Whatever you say to grandma (whatever you type in), she should respond with `HUH?!  SPEAK UP, SONNY!`, unless you shout it (type in all capitals).
    2. If you shout, she can hear you (or at least she thinks so) and yells back, `NO, NOT SINCE 1938!`
    3. To make your program really believable, have grandma shout a different year each time; maybe any year at random between 1930 and 1950.
    4. You can't stop talking to grandma until you shout `BYE`.
- Extend your Deaf Grandma program: What if grandma doesn't want you to leave? When you shout `BYE`, she could pretend not to hear you. Change your previous program so that you have to shout `BYE` three times in a row. Make sure to test your program: if you shout BYE three times, but not in a row, you should still be talking to grandma.
- Leap Years: Write a program which will ask for a starting year and an ending year, and then puts all of the leap years between them (and including them, if they are also leap years). Leap years are years divisible by four (like 1984 and 2004). However, years divisible by 100 are not leap years (such as 1800 and 1900) unless they are divisible by 400 (like 1600 and 2000, which were in fact leap years).
