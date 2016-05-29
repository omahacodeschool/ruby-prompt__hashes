---
title: Hashes
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a Hash?

 A hash is a collection of elements, each of which has a definable index, called key-value pairs.

# What are some examples of information that would be Hashes as opposed to some other data type?

A list of elements that have retrievable attributes would be an example of a hash. As in the Ruby Monk lesson, a list of menu options and their corresponding prices would be a hash.

# How are Hashes and Arrays similar? How are they different?

A hash is like an array in that it is a collection of values, each with an assigned index. In an array, an element's index is an integer; however, in a hash, the index, called the key, can be anything.

# How do you retrieve a particular value from a Hash?

A value can be retrieved from a hash by using its index, or key. In the hash hash = {"color" => "blue", "number" => "five"}, hash["color"] would return the value of the key "color", which is "blue".

# How do you add information to a Hash?

To add information to a hash, a new key is defined and is set equal to a given value. For example, in the above hash, hash["animal"] = "dog" would add the key "animal" to the hash with the value of "dog".

# How would you perform an operation on every element inside a Hash?

Hashes can be iterated over just as arrays can. If the .each method is used, .each will set a variable for both the key and the value. The result must then be passed back into the hash. For example, hash.each do |key,value| hash[key] = value.upcase end would call the .upcase method on each value in the hash and then add those values back into the hash. 

# How would you change the value of a particular element in a Hash?

The value of an element in the hash can be changed the same way that the value can be retrieved. Rather than simply retrieving it though, the key can be reassigned a new value. For example, in the hash above, hash["color"] returns "blue", while hash["color"] = "red" reassigns the value of "red" to the key "color".

# How do you delete an element from a Hash?

The .delete method deletes an element from the hash and receives a given key as an argument to determine which element to delete. For example, hash.delete("number") would remove the pair "number"/"five" from the hash.

# What happens if you try to retrieve an element from a Hash that does not exist in the Hash?

Trying to retrieve an element from a hash that does not exist will return nil.

# How do you determine how many elements are in a Hash?

The .length method returns the number of key-value pairs in a hash.