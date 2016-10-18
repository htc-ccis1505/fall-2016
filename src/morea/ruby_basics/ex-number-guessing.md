---
title: "Number Guessing Game"
published: true
morea_id: ex-number-guessing
morea_type: experience
morea_summary: "Write a simple number guessing game in Ruby."
morea_sort_order: 1
---

# Number Guessing Game
We're going to write a number guessing game in ruby.  

You can get a random number in ruby by using the `rand` function.  If you want a number between 1 and 10 you would use:
{% highlight ruby %}
rand(1..10)
{% endhighlight %}

The game should:

- Ask for the player's name
- Greet the player by name and explain the game
- Ask for the maximum number to select as the secret number
- Pick a secret number at random between 1 and the number entered
- Ask the player (by name) to guess a number
- Tell the player if they guessed correctly
- If they guessed the number correctly, congratulate them for winning and then tell them how many guesses it took for them to win.
- If they did not guess correctly, tell them whether their guess was too high or too low.
