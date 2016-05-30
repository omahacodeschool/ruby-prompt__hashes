---
title: Hashes
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a Hash?

A hash is a collection of elements like an array, but instead of referring to elements by numerical position they are named with a "key" and given value.
A hash can be created using curly brackets and then the key and value pairs listed using the "=>" like this:

    {"Erin" => 24, "Karen" => 25}

Now I have a hash with two elements, "Erin" with a value of 24 and "Karen" with a value of 25.


# What are some examples of information that would be Hashes as opposed to some other data type?

Hashes can be used for any sort of list that has elements that each have a value. Things like inventories listing the number of specified items, or students and their GPAs. This allows us to find information with the key in ways that aren't possible with arrays.


# How are Hashes and Arrays similar? How are they different?

Hashes and arrays are both collections of data and share a number of methods like .length and .each. Hashes have another layer of information contained in them, the named key. This key is used to find certain values instead of using the numerical position in the dat set.


# How do you retrieve a particular value from a Hash?

You can find a value for a key like you would in an array, but in this case the key is specified in the square brackets like this:

    veggies = {"beans" => 300, "bok choy" => 15, "carrots" => 22}
    veggies["beans"]
    
This will return a value of 300. The .fetch method also works to find a value associated with a key.


# How do you add information to a Hash?

To add information you define a new key in square brackets and then use "=" to define it's value like this:

    veggies["onions"] = 11

Now the array contains the key "onions" with a value of 11. 


# How would you perform an operation on every element inside a Hash?

You can perform an operation on each element using the .each method. With .each you can set up a block of code in curly quotes that will be executed on each key/value pair. It might look like this:

    veggies.each { |veg, number| puts "There are #{number} #{veg}."}

The block is contained in the brackets. The vertical slashes create variables, the first one representing the keys and the second representing the values of those keys.
This code will return a string for each key/value pair telling the user how many of each vegetable exists in the array.


# How would you change the value of a particular element in a Hash?

You can change the value of an element in much the same way that you added an element, but this time an existing key is specified and it's value changed with "=".

    veggies["beans"] = 350

Now the key "beans" has a value of 350.

# How do you delete an element from a Hash?

You can delete elements using the aptly named .delete method. By using .delete and specifying the key in parentheses, that key/value pair will be removed from the hash like so:

    veggies.delete("carrots")

Now the hash no longer contains the key "carrots" or its value.


# What happens if you try to retrieve an element from a Hash that does not exist in the Hash?

Now if you were to attempt to retrieve the value of "carrots" the program will return a "nil" because nothing exists with that key in the hash.


# How do you determine how many elements are in a Hash?

Like you would with an array, you can use the .length method to find the number of elements in a hash:

    veggies.length

This will return the number 3.