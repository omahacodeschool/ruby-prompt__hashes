---
title: Hashes
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a Hash?

A Hash is a dictionary-like collection of unique keys and their values. They are similar to Arrays, but where an Array uses integers as its index, a Hash allows you to use any object type.

# What are some examples of information that would be Hashes as opposed to some other data type?

As stated above, Hashes can hold any type of object data. For example: grades = { "Jane Doe" => 10, "Jim Doe" => 6 } 

# How are Hashes and Arrays similar? How are they different?

They are similar in the fact that they both hold indexes of information like a library. The difference is that hashes can hold many more types of data than an array can.


# How do you retrieve a particular value from a Hash?

you would use the command hash.[key]. An example would be: 

elements = {"base"=>"foundation", "pedestal"=>"base"}
  puts elements["base"]
  
  and that will bring back the result "foundation"

# How do you add information to a Hash?

We would replace it by performing this operation:
hash = {:item1 => 1}
hash[:item2] = 2

# How would you perform an operation on every element inside a Hash?

I believe it is similar to that of an array. You would take your elements inside your hash and bundle them under another name, such as Contacts.
You would then type in whatever command you wanted to go with it, like Contacts.delete[David] and that would remove David from out list.

# How would you change the value of a particular element in a Hash?

To replace or change a value in a particular element you would want to use merging. an example would look like:
elements = {"base"=>"foundation", "pedestal"=>"base"}
  added = {"base"=>"non-acid", "salt"=>"NaCl"}
  elements.update(added)

# How do you delete an element from a Hash?

You would delete an element by adding a ".delete()" depending on the item. EX: 
elements = Hash.new()
elements[100] = "a"
elements[200] = "b"
elements[300] = "c"
elements[400] = "d"
elements.delete(100)
That would remove the element[100] from it so if you continued with a element.count it would show that there is 3 instead of 4.

# What happens if you try to retrieve an element from a Hash that does not exist in the Hash?

When you try to get the value of an element that does not exist, the system gives nothing back or displays "nil"

# How do you determine how many elements are in a Hash?

To determine how many elements are in a hash you would type a .count after whatever you labeled your Hash as. 
Example:
elements = Hash.new()
elements[100] = "a"
elements[200] = "b"
elements[300] = "c"
elements[400] = "d"
elements.count

That will bring up a count of 4 elements within the Hash labeled elements.