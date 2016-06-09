---
title: Hashes
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a Hash?

A dictionary like collection of data that pairs unique keys to their corresponding vaules.

# What are some examples of information that would be Hashes as opposed to some other data type?

Keys can be any data type.
Strings and numbers would be the two most common data types. 

I would use hashes to keep track of things like name:number  name:email  name:address
product:price  product:location    x-value:y-value   state:capital  username:password etc


# How are Hashes and Arrays similar? How are they different?

Hashes are special arrays.  
They can be used interchangably, but hashes are easier to maintain and manipulate.
Arrays use integers to index so you have to remember where the information is stored.
Hashes store the information in a less liner fashion so all you have to remember are the keys.



Repsonse:
If I just wanted a list of students I would use an array.  It would be easy to add to the end of and I could maulipulate it
using the array methods. 

If I were to pair information like like a student's name to his/her email, I would use a hash.  
It is much easier to remember a word or name than it is to remember a number or index.

If you want to link name, email, and age it would be best to use an array of hashes.



# How do you retrieve a particular value from a Hash?

Use the [ ] operator.  

hash = {}
hash["wanted_key"]
will return the wanted_value

# How do you add information to a Hash?

The "bracket equals" method.
hash = {}
hash["new_key"]=new_value

# How would you perform an operation on every element inside a Hash?

The best thing to do would be to use an iteration loop.  
You can also the each method.  

# How would you change the value of a particular element in a Hash?

You can just reassign a value to a key.  
The program will use the latter value

# How do you delete an element from a Hash?

Use .delete.  

# What happens if you try to retrieve an element from a Hash that does not exist in the Hash?

The program returns nil.  You can set a different default if desired.


see screen shot on pull request comment



# How do you determine how many elements are in a Hash?

.length returns the number of keys