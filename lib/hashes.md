---
title: Hashes
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a Hash?

A hash is a collection of key-value pairs.

# What are some examples of information that would be Hashes as opposed to some other data type?

Some information that would be stored in a hash would be dictionary definitions, menu items and their prices, as well as names and ages.

# How are Hashes and Arrays similar? How are they different?

Hashes and arrays are similar in that they both store information that can be retrieved. They are different in that elements in an array are only associated with their numerical slot where a value in a hash can be accessed by calling its key.

# How do you retrieve a particular value from a Hash?

You can retrieve a particular value from a hash by calling it's associated key. If the key "Chris" is associated to the value "29", in the hash "names", I could retrieve the value, 29, with names["Chris"].

# How do you add information to a Hash?

You can add information to a hash with the "bracket-equals" method: names["Joe"]= "28"

# How would you perform an operation on every element inside a Hash?

You can perform an operation on every element in a hash using the method "each", which unlike an array, will pass two values (key and value) into the hash.

# How would you change the value of a particular element in a Hash?

You can change the value of an element in a hash like so: names = {"Chris" => 29}, names["Chris"]= 40.

# How do you delete an element from a Hash?

To delete an element from a hash you can use the ".delete" method: names_ages = {"Chris" => 29, "Joe" => 28}; names_ages.delete("Chris")

# What happens if you try to retrieve an element from a Hash that does not exist in the Hash?

By default, if you try to retrieve an element from a hash that doesn't exist, "nil" will be returned.

# How do you determine how many elements are in a Hash?

You can determine how many elements are in a hash with the ".length" method. Using the above hash: names_ages.length yields "2".