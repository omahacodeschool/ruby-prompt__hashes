---
title: Hashes
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a Hash?

A hash is a collection of objects, like an array, but they dont have to be numbers.  Hashes contain a set of 'keys' and 'values', where
the values dont need to be numbers.

# What are some examples of information that would be Hashes as opposed to some other data type?

The information used in a hash would be lists of items, to be set for a given value.  A ranking of different teams and their given value in different
areas, such as strength, speed, debth, etc, or a list of ingredients on a pizza.

# How are Hashes and Arrays similar? How are they different?

Hashes and arrays are both lists, but hashes dont have to use numbers to index them, or describe them, they can be terms or definitions.

# How do you retrieve a particular value from a Hash?

A value from a hash can be retrieved by 'put'ing or 'print'ing the value like a variable.

# How do you add information to a Hash?

A hash is built by defineing the hash, and puting given keys to be equal to or greater than the given value.

# How would you perform an operation on every element inside a Hash?

I am really struggling with this question, and the same question with refference to performing an opperation to every element in an array.

# How would you change the value of a particular element in a Hash?

by referencing the 'key' that you want to change, you can change the 'value' after you have created the hash.  This is my 'pizza hash'
pizza = {'crust' => 'White Flour','Sauce' => 'Tomato Basil','Cheese' => 'Mozzerella',
'Topping_1' => 'Mushrooms','Topping_2' => 'Pepperoni'}
if I wanted to change the type of crust for the pizza, I would:
pizza['crust'] = 'Wheat Flour'

# How do you delete an element from a Hash?

The '.delete' command should delete an element from a hash.  Such as pizza.delete('Topping_1')

# What happens if you try to retrieve an element from a Hash that does not exist in the Hash?

I dont think anything will happen if you havent defined it in the hash.

# How do you determine how many elements are in a Hash?

print hash.size should give you how many elements are in the hash.