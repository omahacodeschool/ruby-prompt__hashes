---
title: Hashes
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a Hash?

A hash is the python form of a dictionary.  They are similar to arrays, but whereas an array uses an integer to index and organize the objects located within it, whereas a hash is more variable.  The keys can use any object value to help organize
the list.  Hashes can help group different items/objects in the list into associations.  Like what I know from python, the key is the sorting, association-making variables that help group, label, and identify the values assigned to them.

# What are some examples of information that would be Hashes as opposed to some other data type?

Since hashes do not store the items in a numbered list, so if you need the data stored in a specific order, so that it can be called by referencing a specific number in that sequence, then hashes would not be useful.  They can group and organize data/objects,
and make it so that items can be called without havinig to memorize their specific number in the ordered list or array.  Hashes stor named data, so one can use key data and sorting to do a lot of useful things with the data.  A type of data that can 
benefit from the use of hashes is counting data, as it can store amounts of a certain type of item (as opposed to arrays).

# How are Hashes and Arrays similar? How are they different?

Some of this response could be found in the previous answer above, but I'll try to repeat as much here.  Both arrays and hashes are collections of information, stored in a form of repository.  The differences come mainly from how that data is stored, and how that data can be used or called.
Arrays store the data/objects in a specific order, and particular items can be called by utilizing the number of the item in that list (beginning with zero).  Hashes have keys, which are unique names that can be used to identify values.  The keys can be used to help do a variery of things, like 
organize a count of like items, or categorize items into desired groups, etc.  Hashes have much more variety in terms of what they can offer.
# How do you retrieve a particular value from a Hash?

A particular value from a hash is retrieved by using the key for that value.  For instance, if this is our hash:  grades = { "Mike Ducey" => "A", "Pat Ducey" => "B+" } , you reference the hash like an array, but instead of specifying the number of the item, you use the key.  So, in this case, if I write grades["Mike Ducey"], I shall get => A as a response.
# How do you add information to a Hash?

This is done by using the "bracket-equals method" (https://github.com/learn-co-curriculum/hash-overview-readme).  That is, if you have a hash and you want another key in the hash, you can write the name of the key in the brackets and the value after the equal sign.  I'll add a grade to my grades hash: grades["Kevin Ducey"] = A-
# How would you perform an operation on every element inside a Hash?

This is achieved by using the each function.  If you want to change each value, you use something of the form: grades.each do |x| where x is the change to be done using code.
Here is the function I wrote after some help!

grades = {"Alex" => 90, "Sumeet" => 98, "Khalil" => 85}
grades.each_pair do |x,y|
puts y + 5
puts " " 
end

# How would you change the value of a particular element in a Hash?

This is done via utilizing the same sort of method as assigning a new key/value pair.  So, it is basically an overwriting of a value.  I could write grades.update("Pat Ducey") => "C+"  and that would be the new value for the key "Pat Ducey"

# How do you delete an element from a Hash?

To delete a particular element from a hash, a user will use the delete function and put the key that identifies the element in parentheses.  For instance, if I were to write grades.delete("Mike Ducey"), it would remove the key-value pair of "Mike Ducey" +> A from the grades hash.

# What happens if you try to retrieve an element from a Hash that does not exist in the Hash?

If you use a key that has no corresponding element, it will return the default value.   The default can be changed to represent what the default value is.  So, in our grades hash, we could write grades.default = "That student does not exist"  So if I went to call grades["David Bowie"] from the grades hash, it would return That student does not exist.

# How do you determine how many elements are in a Hash?

The length function would give the number of key-value pairs (and then supposedly the number of elements!) I'm a bit vague on this, but I think from what I've learned that you can use count = hash_name.le.
That count will be the number of elements in that hash.