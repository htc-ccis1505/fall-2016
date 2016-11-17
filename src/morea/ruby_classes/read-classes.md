---
title: "Ruby: Classes"
published: true
morea_id: read-classes
morea_summary: "Chapter 8 - Classes."
morea_type: reading
morea_sort_order: 2
morea_labels:
 - ruby
 - textbook
---

# {{ page.title }}
Read through Chapter 10 in the printed textbook, or Chapter 9 in the online [Learn to Program](https://pine.fm/LearnToProgram/chap_09.html), which covers how to work with classes in Ruby.

As you read through the text, make sure you are sitting at your computer and trying the commands in interactive ruby from the shell.  

## Notes on the Reading
### Using Objects
We've been working with objects in Ruby, Integer, String, Array, etc., without really focusing on the fact that they're objects.  The main point has been that you're calling methods on objects with the *variable dot method-name* notation.

{% highlight ruby %}
name = "Hello"
length = name.length
{% endhighlight %}

In the example above, `name` is a variable that holds a Ruby object, a String.  When you enter `name.length` you are using the dot after the variable name to access a method or property that is a part of that object.  In the above example, you're getting the String's `length`.

### Time, Hash & Other Classes
I don't expect you to remember anything specific about the Time class.  

However I do expect you to know and understand how to use the Hash class.  The Hash class can be very handy, and there are objects similar to the Hash found in most programming languages.  They are sometimes called maps or dictionaries.  A Hash is like an Array in many ways, but instead of accessing items by position, you use a "key" or a name to access the value.

I will not expect you to know all of the classes in Ruby, only the ones discussed in the reading and used in our labs.  However being aware of how to find and use other Ruby classes may be valuable to you outside of the scope of this course.  You can find information on Ruby classes from the [Ruby Docs](http://ruby-doc.com/docs/ProgrammingRuby/html/builtins.html) site.

### Custom Classes
For this course, we will focus more on making our own classes, so in the reading, focus on the sections for __Creating Classes__ and __Instance Variables__.

In the Dragon example, notice that the discussion after the code talks about what the keyword __private__ is doing in the code.  There are some methods that are public and some are private.  Private methods allow us to keep the internal workings of our object code hidden from code outside of the object itself.  We've talked about this idea of hiding things before, right?  Objects also provide a means for abstraction.  

## Review Questions

- What Ruby classes have you learned so far?
- How is a Hash different from an Array?  How are they similar?
- How do you create a new class?
- What is an instance variable?  How is it different from the variables we used before?
- What character is used at the start of a variable name to indicate it is an instance variable?
- What method is called when a new object is created?
- What is the difference between a class/object and an instance of a class?
- Why would you make a method on a class private?  
- Give an example of a class, discussing instance variables and public & private methods.
- How do the computational thinking concepts we've discussed apply to objects?  (I mentioned abstraction above, but could generalization and/or composition/decomposition fit as well?)

## Try it!
Do the practice exercises from the end of the chapter.

Use Ruby to:

- Make an OrangeTree class. It should have a  height method which returns its height, and a  oneYearPasses method, which, when called, ages the tree one year. Each year the tree grows taller (however much you think an orange tree should grow in a year), and after some number of years (again, your call) the tree should die. For the first few years, it should not produce fruit, but after a while it should, and I guess that older trees produce more each year than younger trees... whatever you think makes most sense. And, of course, you should be able to countTheOranges (which returns the number of oranges on the tree), and pickAnOrange (which reduces the @orangeCount by one and returns a string telling you how delicious the orange was, or else it just tells you that there are no more oranges to pick this year). Make sure that any oranges you don't pick one year fall off before the next year.
- Write a program so that you can interact with your baby dragon (from the text code examples). You should be able to enter commands like  feed and walk, and have those methods be called on your dragon. Of course, since what you are inputting are just strings, you will have to have some sort of method dispatch, where your program checks which string was entered, and then calls the appropriate method.
