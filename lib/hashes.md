---
title: Hashes
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

•	What is a Hash?
o	A hash is a dictionary-like collection of unique keys and their values.  Hashes are very similar to arrays but instead of arrays using integers as its index, a hash allows you to use any object type. 

•	What are some examples of information that would be Hashes as opposed to some other data type?
o	An example of using hashes is food prices. With hashes you can do search on a string such as “pizza” and find the integer value it’s been assigned for the price.
    With arrays you can’t do searches by string types only by integers for its index. 
    
•	How are Hashes and Arrays similar? How are they different?
o	Both hashes and arrays use list like system to store information. The differences are arrays must use integers for its index but hashes allow you to use any type of object for it's key.  

•	How do you retrieve a particular value from a Hash?
o	You would call it by the key such as the following array_here [“pizza”]

•	How do you add information to a Hash?
o	To add new information to existing array you’ll do the following
o	Array_here [“hamburger”] = 8

•	How would you perform an operation on every element inside a Hash?
o	You would perform the each method, such as 
o	array_here.each do | x, y |
o	end

•	How would you change the value of a particular element in a Hash?
o	You would call the key of the value you want to change and assign the new value such as array_here[“pizza”] = 12 

•	How do you delete an element from a Hash?
o	You can call the delete method such as array_here.delete(“pizza”)

•	What happens if you try to retrieve an element from a Hash that does not exist in the Hash?
o	 It would return nil response back. 

•	How do you determine how many elements are in a Hash?
o	You would use the length method such as array_here.length. 