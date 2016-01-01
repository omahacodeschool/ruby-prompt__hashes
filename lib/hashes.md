---
title: Hashes
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a Hash?

A hash is an unordered list of key value pairs.  Other languages call it a dictionary sometimes and that's not such a horrible way to think about them.  It's similar to an array, but the key value pairs are unique and use that for indexing, as opposed ot an array which is indexed using integers.  

# What are some examples of information that would be Hashes as opposed to some other data type?

Well, as mentioned, other languages call hashes dictionaries.  Matching a word to a definition isn't so far off from matching a key to a value.  You could use a hash to keep track of paired bits of data, e.g., a phone book pairing names to numbers, a gradebook pairing students to their grades, or keeping inventory pairing products with their quantities or prices.

# How are Hashes and Arrays similar? How are they different?

Well, superficially, they're indicated differently in ruby.  Whereas brackets [] were the order of the day with arrays, hashes are indicated by braces {}.  So, if an array would look like array_1 = [1,2,3,4,5] whereas a hash would look like hash_1 = { "Suzie" => 10, "Calvin" => 2, "Hobbes" => 7}  Beyond that, as mentioned, they're indexed differently.  An array is indexed using integers, so if you want to call up a particular element in an array, you'd indicate its position,e.g., in array_1 = [1,2,3,4,5] each item has a position number and to call up that item you look up that position.  For a hash, it's indexed via the unique keys, thus in hash_1 = ["Suzie" => 10, "Calvin" => 2, "Hobbes" => 7} you'd indicate the key to call up its corresponding value. So, they're similar to one another in that they're both collections of data, but that data is structured and retrieved in different manners and better suited to different tasks.

# How do you retrieve a particular value from a Hash?

To retrieve a particular value from a hash, you'd call up it's key.  So in hash_1, if you wanted to call up the value associated with "Suzie" you'd say hash_1["Suzie"] and it should return 10.

# How do you add information to a Hash?

You should be able to add a new key value pair by entering them in the format hash[key] = value, where "hash" is whatever it is you've named your hash.

# How would you perform an operation on every element inside a Hash?

You'd use the each method.  So, if you had a hash wherein you wanted to increase all your values (assuming they're integers) by a value of 1, you could type something like hash.each do |key, value| and specify in the block hash[key] = value  + 1.  It's worth noting that this change is superficial.  It doesn't actually change the values in the hash, it just performs a given action or set of actions on them.

# How would you change the value of a particular element in a Hash?

To change a given value in an element of a hash, you could call up its key and assign it a new value.  So, if the hash is hash = {"a" => 1, "b" => 2, "c" => 3} you could say hash["a"] = 2.

# How do you delete an element from a Hash?

You'd use the delete method so, if you wanted to remove a particular key and its associated value from a given hash you'd say something in the format hash.delete(key) this will remove both key and value.  If you wanted to just nuke the whole thing you could use the clear method.

# What happens if you try to retrieve an element from a Hash that does not exist in the Hash?

It'll return the default value, nil.  So, if you have a hash with three key value pairs, hash = {"a" => 1, "b" => 2, "c" => 3} and tell it puts hash["z"] it'll just return nil.

# How do you determine how many elements are in a Hash?

Well, as before, there are built in methods for this.  To determine the number of elements in a given hash you can use the count, length, or size methods.  So, in the hash mentioned in the previous question, were you to say hash.length, hash.size, or hash.count it would return 3.  Though it's probably outside the scope of our interests for general use, one article I found on the subject indicated that of the three methods, count, because it had to travers the entire enumerable, which could be quite large, you might encounter some speed issues and thus should probably use length or size for most purposes.  Also, and this sounded like something of an aesthetic choice, the author of that particular article stated that he preferentially uses length with things like strings which actually have a length and size which don't really have a length per se.  Although, there wasn't anything noted as being different about what the two methods actually do.