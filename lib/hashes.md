---
title: Hashes
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a Hash?

A Hash is a collection of key-value pairs very similar to a dictionary. It are similar to Arrays, but where an Array uses integers as its index, a Hash allows you to use any object type.

# What are some examples of information that would be Hashes as opposed to some other data type?

You would use Hashes when you want to be able to use different elements/categories to index your values. 

# How are Hashes and Arrays similar? How are they different?

They are similar since they are both use to store a collection of data.

They are different because arrays store the data in a index-numbered list whereas hashes store data with key-value pairs by using strings, numbers, or symbols. 

# How do you retrieve a particular value from a Hash?

By calling the values key. For example hash = {"key" => "value", "another_key" => "another value"}

# How do you add information to a Hash?

my_hash_name[new_key_name]= new_value

# How would you perform an operation on every element inside a Hash?

my_hash.each do |key, value|
    my_hash[key] = new_value (whatever edit I want to make for every value)

# How would you change the value of a particular element in a Hash?

my_hash_name[particular_key]= new_value

# How do you delete an element from a Hash?

my_hash_name.delete(element)

# What happens if you try to retrieve an element from a Hash that does not exist in the Hash?

The operation returns nil.

# How do you determine how many elements are in a Hash?

my_hash_name.count