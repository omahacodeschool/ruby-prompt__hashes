---
title: Hashes
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a Hash?

A Hash is a collection of key-value pairs. 

# What are some examples of information that would be Hashes as opposed to some other data type?

Hashes are useful for storing information that is related such as a teacher's grade book, storing the students names with their grades, or a construction manifest, storing the supplies needed with how much of each supply needed. 

# How are Hashes and Arrays similar? How are they different?

Hashes and arrays are similar in that they both store information that can be appended to and later retrieved. They are different in the way that they are indexed. In an array each element is stored as an integer in order starting with zero, whereas in a Hash, each element is stored as a value associated to a related key.

# How do you retrieve a particular value from a Hash?

Much like with an array you can retrieve a particular value from a Hash using the [] operator. In order to do so, the key of the value we are looking for should be enclosed within the square brackets.

# How do you add information to a Hash?

In order to add information to a Hash you need to define both a new key along with it's associated value. For example, to add Susie Queue's grade to the teacher's gradebook hash named "gradebook" the command would be 'gradebook["Susie Queue"] = 86'

# How would you perform an operation on every element inside a Hash?

Again, like with array's in order to perform an operation on every element inside of a Hash you can call the each method. 

# How would you change the value of a particular element in a Hash?

In order to change the value of a particular element in a Hash, you could create a duplicate of the particular key of whose value you were looking to change and assign it the new value. 

# How do you delete an element from a Hash?

Much like with array's, the delete method can be called to delete a specific key and it's associated value. 

# What happens if you try to retrieve an element from a Hash that does not exist in the Hash?

If you try to retrieve an element from a Hash that does not exist in the Hash, ruby will return nothing. 

# How do you determine how many elements are in a Hash?

Again, with hashes, the length method can be called in order to return the number of key-value pairs in the Hash.