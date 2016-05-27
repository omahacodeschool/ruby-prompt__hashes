---
title: Hashes
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a Hash?

A hash is defined by curly brackets {} and can be viewed as a form of an array
except the order or list of values are not important with hashes as it is with arrays.

# What are some examples of information that would be Hashes as opposed to some other data type?

When calling for a value within a hash, a key must be used instead of an integer
(unless an integer was used as a key).

# How are Hashes and Arrays similar? How are they different?

As mentoined before, hashes use keys to call for their stored values unlike 
arrays. Both still are meant to store information and have methods of adding values.

# How do you retrieve a particular value from a Hash?

Every value has an assigned key. A hash hash_name{key} will produce the value 
assigned to that key.

# How do you add information to a Hash?

Because order doesn't matter in hashes, simply using hash_name{newkey}=newvalue 
will add that information.

# How would you perform an operation on every element inside a Hash?

Using .map can change the hash to one with different values compared to the originals.

# How would you change the value of a particular element in a Hash?

A simple redefinition statement would work. If a key "A" originally was 15 in 
hash_name then by using hash_name["A"]= 16 will change the original to 16.

# How do you delete an element from a Hash?

hash_name.delete("key") would be a command to delete an element from a Hash.

# What happens if you try to retrieve an element from a Hash that does not exist in the Hash?

The response from the command would be nil

# How do you determine how many elements are in a Hash?

hash_name.length would answer how many elements are in a Hash.