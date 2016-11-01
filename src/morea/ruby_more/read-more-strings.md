---
title: "Ruby: More Strings"
published: true
morea_id: read-more-strings
morea_summary: "More things you can do with Strings in Ruby."
morea_type: reading
morea_sort_order: 1
morea_labels:
 - ruby
---

# {{ page.title }}
{{ page.morea_summary }}

## Review: Strings
Several methods for Strings were introduced earlier in the reading:

- reverse
- length
- upcase
- downcase
- swapcase
- capitalize

Remember that these methods do not modify the string you call them on, they create a new string.

{% highlight ruby %}
word = "programming"
puts "The word is " + word
puts "Reversing the word gives: " + word.reverse
puts "But, the word is still " + word
{% endhighlight %}

If you really want the variable to reflect the change, you must reassign it to the output, but then you lose the initial value:
{% highlight ruby %}
word = "programming"
puts "The word is " + word
word = word.reverse
puts "The word is now reversed: " + word
{% endhighlight %}

## Get a single letter
You can also get a single letter from a String using syntax similar to array notation:

{% highlight ruby %}
word = "programming"
puts "The first letter of the word is " + word[0]
puts "The last letter of the word is " + word[word.length-1]
{% endhighlight %}


## Iterators for Strings
We've seen how iterators can be used with an array, but there are also iterators that can be used with strings.

{% highlight ruby %}
word = 'programming'

word.each_char do |letter|
    puts letter
end
{% endhighlight %}

Since we can also get a single letter from a string much like we would from an array, this is similar to the following for loop:

{% highlight ruby %}
limit = word.length
for counter in 0..limit
  puts word[counter]
end
{% endhighlight %}

There always seems to be more than one way to do the same thing in programming, doesn't there.

## Split a String
We've seen how to join elements of an array into a String earlier in the reading:

{% highlight ruby %}
fruits = ['Apple', 'Banana', 'Cherry', 'Date']
puts fruits.join(', ')
{% endhighlight %}

We can also break a string into an array using the split method:
{% highlight ruby %}
fruit_string = "Elderberry, Fig, Grape"
more_fruit = fruit_string.split(', ')
puts more_fruit.to_s
{% endhighlight %}

We can also break a word into an array of letters:
{% highlight ruby %}
letters = word.split('')
puts letters.to_s
{% endhighlight %}

## Try It!

- Write a while loop to display each letter in a word one at a time.
- Write method to display each letter in a word backwards, one at a time.
- Write a method to reverse a string without using the built-in string reverse method.
- Write a method that takes two words as input and returns the position of the first letter that is different between them.  If the words are the same, return -1 (since 0 would indicate the first letter).
- Write a method to translate "old-school" Roman numerals to a number.  
