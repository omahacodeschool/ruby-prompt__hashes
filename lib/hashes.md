---
title: Hashes
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a Hash?

A hash is another type of collection, similar to an array. 
hash data is not stored in rows, and slots can be referenced by any object type (not just a number).

# What are some examples of information that would be Hashes as opposed to some other data type?

Hashes are ideal for data where you would want to categorize items as well as store them. 
Any data type that would lend itself to a table (vs. a list) - like a class roster with contact information - would be an appropriate hash.
Also, because hash data is stored in pairs, it would be a good tool for building a dictionary.

# How are Hashes and Arrays similar? How are they different?

They are similar in that they both are data collections. 
In an array, data elements are stored in a row in a numbered slot. It is stored in a consistent order. You must know the data's location to retrieve it.
In a hash, data elements are stored in unique pairs - all elements are stored with a logically associated key. It is not stored in a consistent order. It is retrieved by calling the key.

# How do you retrieve a particular value from a Hash?

To retrieve information within a hash, you use the key value for the information you want.
As an example, in a hash that contains the members of the band The Beatles, the code might look like:
  The_Beatles['Guitar'] #=> John Lennon

# How do you add information to a Hash?

To objects to a hash, we use the bracket-equals method, which might look like:
  The_Beatles['Bass'] = "Paul McCartney"

# How would you perform an operation on every element inside a Hash?

The most convenient way to perform an operation on every element in a hash would be to use the each_pair method:
  The_Beatles.each_pair{ |key,val| puts key.downcase, val.downcase }

We can also use the .each_key or .each_value method, to focus on just that element within the hash pair.

# How would you change the value of a particular element in a Hash?

To change a particular element within a hash, we could simply rewrite the value attached to the associated key.
  The_Beatles = {"Guitar" => "John Lennon", "Bass" => "Paul McCartney", "Drums" => "Pete Best"}
  The_Beatles["Drums"] = "Ringo Starr"

# How do you delete an element from a Hash?

To delete an element from a hash, we could use the .delete(key) method
  The_Beatles = {"Guitar" => "John Lennon", "Bass" => "Paul McCartney", "Drums" => "Pete Best", "Bass2" => "Stuart Sutcliffe"}
  The_Beatles.delete("Bass2")

# What happens if you try to retrieve an element from a Hash that does not exist in the Hash?

As with the array, retrieving an element that does not exist returns a nil value, expressed as a blank space in a list.
You can also set a default value instead of the nil. 

# How do you determine how many elements are in a Hash?

We can use the .length method to return the number of key,value pairs within the hash.