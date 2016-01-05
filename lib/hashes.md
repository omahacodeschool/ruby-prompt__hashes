---
title: Hashes
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a Hash?

An unordered collection of unique keys and their values.

# What are some examples of information that would be Hashes as opposed to some other data type?

lists that require to be broken out into subcategoires that do not require a particular order as opposed to just lists that fall into one category.  I.E. 

student_ages = {
    "Jack" => 10,
    "Jill" => 12,
    "Bob" => 16
}


# How are Hashes and Arrays similar? How are they different?

Arrays allow you to make an ordered list.  Hashes allow you to make an unordered list (keys) but with details/definitions (values).

# How do you retrieve a particular value from a Hash?

Write the name of the object and follow it with square brackets [] and inside the brackets write the key. If the key is a string use quotation marks.

# How do you add information to a Hash?

hash.merge! As far as I can tell it doesnt alter the original hash but creates a new one using the previous hash and the new hash.  It took me 2 hours to find this answer...
hash = {"a" => 1} hash.merge!("b" => 2, "c" => 3)
# How would you perform an operation on every element inside a Hash?

name.each do |key/value|

# How would you change the value of a particular element in a Hash?

hash.merge! works for this as well. Using the same code as above hash = {"a" => 1} hash.merge!("b" => 2, "c" => 3)
 you can just add hash.merge!("b" => 4) and it will return {"a"=>1, "b"=>4, "c"=>3]
# How do you delete an element from a Hash?

Hash.delete (key)

# What happens if you try to retrieve an element from a Hash that does not exist in the Hash?

nil is returned

# How do you determine how many elements are in a Hash?

hash.count