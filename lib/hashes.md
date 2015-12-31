---
title: Hashes
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a Hash?

Hashes are sort've like arrays, in the sense that tehy are a collection of keys and their values. 
 At a very basic level, hashes look like:
HASHTHING = { "KEY" => KEYVALUE, "KEY2" => KEY2VALUE }

# What are some examples of information that would be Hashes as opposed to some other data type?

menus, inventory, a class roster and each child's emergency contact, user scores, etc. 

# How are Hashes and Arrays similar? How are they different?
SAME: Both can store large amounts of list data and use indexes to identify elements in the list. 

DIFFERENT: Hashes and arrays are different, as hash indexes use object type
rather than integers. Hashes also can contain more data an an array, as they store both the key and a corresponding value for that key.
In arrays, the key and value are one and the same. 

# How do you retrieve a particular value from a Hash?
Enclose the key in the [ ] operator. EXAMPLE:
food = {"tacos" =>2, "more tacos" =>2, "all you get is tacos" =>2}
food["tacos"]       #=> 2

# How do you add information to a Hash?
You would select the hash, enlocse the new key in brackets after it, and then set the value. EXAMPLE:

food = {"tacos" =>2, "more tacos" =>2, "all you get is tacos" =>2}
food["still tacos"] = 2
puts food       #=> {"tacos"=>2, "more tacos"=>2, "all you get is tacos"=>2, "still tacos"=>2}


# How would you perform an operation on every element inside a Hash?

use the .each method with a do iteration. EXAMPLE:
food = {"tacos" =>2, "more tacos" =>2, "all you get is tacos" =>2}
food.each do | item, price |
    puts "#{item} costs: #{price}"
end                  #=> tacos costs: 2
                         more tacos costs: 2
                         all you get is tacos costs: 2
# How would you change the value of a particular element in a Hash?

Select the hash, followed by the key enclosed in brackets, and then set a new value. 
food = {"tacos" =>2, "more tacos" =>2, "all you get is tacos" =>2}
food["still tacos"] = 2
food["tacos"]=3
puts food           #=> {"tacos"=>3, "more tacos"=>2, "all you get is tacos"=>2, "still tacos"=>2}

# How do you delete an element from a Hash?

To delete an element from a hash, use the .delete method. EXAMPLE
food = {"tacos" =>2, "more tacos" =>2, "all you get is tacos" =>2}
food.delete("tacos")
puts food           #=> {"more tacos"=>2, "all you get is tacos"=>2}

# What happens if you try to retrieve an element from a Hash that does not exist in the Hash?

If you try to retrieve a non-existant element from a hash it returns nil. EXAMPLE
food = {"tacos" =>2, "more tacos" =>2, "all you get is tacos" =>2}
food["not tacos"]               #=> nil

# How do you determine how many elements are in a Hash?

Use the .length method to determine how many elements are in a hash. EXAMPLE:
food = {"tacos" =>2, "more tacos" =>2, "all you get is tacos" =>2}
food.length             #=> 3