---
title: "Ruby: More Methods"
published: true
morea_id: read-ruby-lib-methods
morea_summary: "Chapter 6 - More About Methods"
morea_type: reading
morea_sort_order: 1
morea_labels:
 - ruby
 - textbook
---

# {{ page.title }}
Read through Chapter 6 in the printed textbook, or Chapter 5 in the online [Learn to Program](https://pine.fm/LearnToProgram/chap_05.html), which introduces Ruby built-in methods for strings, more math stuff, and random numbers.

As you read through the text, make sure you are sitting at your computer and trying the commands in interactive ruby from the shell.  

## What must you remember?
When working in text based languages, at some point you've got to commit methods to memory so that you remember exactly what they are called and what input is required.  While it is not required that you memorize every method available in Ruby, you'll need to remember methods introduced in the reading and in-class, unless it is documented otherwise.  

{% include alert.html type="note"
      content = "If you have trouble remembering the methods we learn, it may be a good idea to make a list for your test notes."
%}

For this chapter in the text, pay particular attention to these string methods discussed:

- reverse
- length
- upcase
- downcase
- swapcase
- capitalize

These are unlikely to be on a test or quiz, but might be handy in a project:
- center
- ljust
- rjust


The additional math operators for exponent ** and modulus % may also come in handy.

You'll definitely want to remember the rand method. Remember that if you give it only one number, it will not give you that number randomly.  It is a value from 0 up to but not including the number given.

The Math object is also worth noting as it is a just a little different.  `Math` is an object much like a string is an object. In the earlier examples we were calling methods on variables:

{% highlight ruby %}
name = 'Buffy'
puts name.upcase
{% endhighlight %}

In the Math examples, we're using the Math object in front of the . before the name of the method, instead of a variable.  

{% highlight ruby %}
Math.sqrt(16)
{% endhighlight %}

The only things from the Math object you may need to know are PI (a constant - a value that does not change) or the `sqrt` method.

## Review Questions

- Why do some methods have () after the name and others do not?
- How could you find out how many letters are in a word?  Will this work no matter what or are there things that could cause it to give an incorrect answer?
- How do I get a random number between 0 and 10 in Ruby?
- What could you do if you wanted a random number between 1 and 10?  (There is a way to specify a range, but how could you do it with the method shown in the book?)


## Try It!
Write the Angry Boss program as discussed in the text.

  1. It should rudely ask what you want.
  2. Whatever you answer, the Angry Boss should yell it back to you, and then fire you.

For example, if you type in `I want a raise.`, it should yell back `WHADDAYA MEAN "I WANT A RAISE."?!?  YOU'RE FIRED!!``
