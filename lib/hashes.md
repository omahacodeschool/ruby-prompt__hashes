---
title: Hashes
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a Hash?

A hash is a collection of information, similar to an Array.  Unlike an array which store information as a list, a Hash stores information in key-value pairs.  Information in a hash can be retrieved
by refering to its key.
# What are some examples of information that would be Hashes as opposed to some other data type?

If someone wanted to store the prices of goods at store they could use a hash.
ie.  merchandise_cost = {
        "Gloves" => 2,
        "Boots" => 6,
        "Coats" => 17,
    }
This is a more organized method of storing information than if I tried to store the same information as an array. 
i.e.  merchandise_cost ["Gloves", 2, "Boots", 6, "Coats", 17]

Because information in an array is stored as a list it is more difficult to retrieve the cost of gloves without already knowing where in the index
the cost of gloves is located.

# How are Hashes and Arrays similar? How are they different?

Hashes and arrays are similar in that they both store information as an object.  An array stores information as a list, where each element in the array is automatically
assigned to a number based on where it's location in the array.  However, a hash stores information as pairs of keys and values, and we decide these pairings.  This allows for us to have
more control over the organization of the hash, and for more complex collections of information.

# How do you retrieve a particular value from a Hash?

To retrieve a value from a hash use [].  Ruby will retrieve the value associated with whatever key is typed inside the [].
If we wanted to retrieve the value for boots in the above array we would type: merchandise_cost["Boots"]

# How do you add information to a Hash?

To add information to a hash we would again use [].  If I wanted to add socks to the merchandise_cost array I would type:
merchandise_cost["Socks"] = 1

# How would you perform an operation on every element inside a Hash?

Like an array, to perform an operation over every element inside a Hash we would use the .each method.  If we wanted to use Ruby to 
return the name of the merchandise and its cost we could type something like:

merchandise_cost= { "Gloves" => 2, "Boots" => 6, "Coats" => 17 }
merchandise_cost.each do |item, cost|
    puts "#{item}: $#{cost}" 
end


# How would you change the value of a particular element in a Hash?

To change the value of a particualr element in a Hash we would again use [].
If I wanted to raise the price of Boots to 8 I would type:

merchandise_cost["Boots"]=8

# How do you delete an element from a Hash?

.delete() will delete the key-value pair for whatever key is placed inside the () and then return the value for what was removed.  For example, if I wanted to remove "Gloves" from the merchandise_cost
hash I would type:  merchandise_cost.delete("Gloves") 
and Ruby would return 3.

# What happens if you try to retrieve an element from a Hash that does not exist in the Hash?

Ruby will return "nil" if you try to retrieve an element that does not exist in the hash.

# How do you determine how many elements are in a Hash?

Similar to an array, to determine the number of key-value pairs in an array use .length.  
i.e. merchandise_cost.length  would return a value of 3. 