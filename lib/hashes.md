---
title: Hashes
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a Hash?

A Hash is a collection of key-value pairs.

# What are some examples of information that would be Hashes as opposed to some other data type?

Any kind of information that has a unique value that is associated with it.

# How are Hashes and Arrays similar? How are they different?

An array is an ordered list that you can call to. Hashes are a collection of paired information. They're not about order but about what info is paired with what.

# How do you retrieve a particular value from a Hash?

You call its key.

# How do you add information to a Hash?

Hashes use the "bracket-equals" [] method to add data.

hash = {
    "apple": "red",
    "pear": "green",
    "banana": "yellow"
  }
hash[:peach] = "peach"

# How would you perform an operation on every element inside a Hash?

Using the .each method. 

hash = {
  "apple": "red",
  "pear": "green",
  "banana": "yellow"
}

hash.each {|key, value| puts "This #{key} is so tasty!" }

returns This apple is so tasty! This pear is so tasty! This banana is so tasty!

# How would you change the value of a particular element in a Hash?
Using the [] method

hash = {
    "apple": "red",
    "pear": "green",
    "banana": "yellow"
  }
hash[:apple] = "peach"

returns {:apple=>"peach", :pear=>"green", :banana=>"yellow"}

# How do you delete an element from a Hash?

Using .delete method follow by the element you wish to be deleted in ().

hash = {
    "apple": "red",
    "pear": "green",
    "banana": "yellow"
  }
hash.delete(:apple)

# What happens if you try to retrieve an element from a Hash that does not exist in the Hash?

It will return a default value or if no default is set it returns nil.

# How do you determine how many elements are in a Hash?

Using .length method 

hash = {
    "apple": "red",
    "pear": "green",
    "banana": "yellow"
  }
hash.length

returns 3