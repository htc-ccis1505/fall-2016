---
title: "Ruby: More Iterators"
published: true
morea_id: read-more-iterators
morea_summary: "More ways to iterate in Ruby code."
morea_type: reading
morea_sort_order: 1
morea_labels:
 - ruby
---

# {{ page.title }}
{{ page.morea_summary }}

## Review: Each Iterator
The each iterator was introduced earlier in the reading:

{% highlight ruby %}
fruit = ['Apple', 'Banana', 'Cherry', 'Date']

fruit.each do |item|
  puts item
end
{% endhighlight %}

This iterator is handy if you want to do something to each item in an array, but do not care what position the item is in.  

## Each with Index
Often however, you'll care what the index is.  Ruby also has an iterator that gives you the index:

{% highlight ruby %}
fruit.each_with_index do |item, index|
  puts "Item " + index.to_s + " is " + item
end
{% endhighlight %}


## For Loop
Many programming languages make use of for loops.  Ruby programmers tend to prefer the iterators, but a more traditional for loop is also available.

{% highlight ruby %}
limit = fruit.length
for counter in 0..limit
  puts fruit[counter]
end
{% endhighlight %}


## Try It!

- Write a while loop to display each item in an array one at a time.
- Write a method that returns a list with only the even numbered items from an original list.
