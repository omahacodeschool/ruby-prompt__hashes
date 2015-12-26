---
title: Hashes
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a Hash?

A hash is a group of items in which each item has an attribute or value stored along with it.

# What are some examples of information that would be Hashes as opposed to some other data type?

Anything that has a value beyond its own name (as far as I know now, these are usually numerical values)--examples include price lists, quantities of attendees for a group of events, run times of various programs, etc.

# How are Hashes and Arrays similar? How are they different?

Hashes and arrays are similar in that they're both a group of items that will be either listed or sorted together. While arrays are simply a list of names, items, or numbers, hashes include more information, as each item can have an additional value attached to it.

# How do you retrieve a particular value from a Hash?

hashname ["itemname"] will call the value of that item.

# How do you add information to a Hash?

hashname ["itemname"] = itemvalue

# How would you perform an operation on every element inside a Hash?

This calls for an .each do operation--this is the example that rubymonk.com gives to raise the menu prices by 10%:
restaurant_menu = { "Ramen" => 3, "Dal Makhani" => 4, "Coffee" => 2 }
restaurant_menu.each do |item, price|
  restaurant_menu[item] = price + (price * 0.1)
end

I didn't get this code right when I was attempting it for myself, but after seeing their cheat solution, it makes sense.

# How would you change the value of a particular element in a Hash?

Using the same code as two questions above, but using an existing item instead of adding a new one: hashname = ["itemname"] = itemvalue.

# How do you delete an element from a Hash?

Using the .delete command-- I used hashname.delete("itemname").

# What happens if you try to retrieve an element from a Hash that does not exist in the Hash?

The program will return 'nil'.

# How do you determine how many elements are in a Hash?

The command .length works here: restaurant_menu.length returns '3' in this case.