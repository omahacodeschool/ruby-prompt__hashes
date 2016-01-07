---
title: Hashes
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. 
We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a Hash?

A Hash is an array that can use any data object as an index, or in hash terms, a KEY. 

# What are some examples of information that would be Hashes as opposed to some other data type?

The custom-made keys in a hash make referencing elements easier to remember than in the numbered array, and in reading about them,
it appears that hashes can do anything an array can. 
The fact that any data object can be used to reference the hash's key makes the position within the list both unimportant and easy to locate. 
The keys in a hash will remain the same no matter what is changed about the other elements. 
A dictionary entry, for example, could be dict = ["Aardvark", "Acidophilus", "Advertising"]
But it wouldn't make sense to put all of these into an array, then have to search by index to find, say, "Quasar".
It would be much easier to just have the hash element:

hsh["Quasar"] = "Really, really bright thing that is very, very far away" 

# How are Hashes and Arrays similar? How are they different?

Hashes and Arrays are both collections, though hashes use curly brackets around elements, 
and the programmer must assign a key to each value in a hash. 
In an array, the key (or Index) is chosen by the order of the elements (ie, 0, 1, 2). 
When a key is chosen for a value in a hash, the other elements have no bearing on that key, as they do in an ordered array. 

# How do you retrieve a particular value from a Hash?

A hash uses the brackets like with an array:

puts hsh["The meaning of life, the universe, and everything"]
#=>42

# How do you add information to a Hash?

Add information to a new hash using the "hash rocket" =>
Use brackets to add more information to the existing hash, like in an array.

Ex:

hsh = {"Horse" => "Breakfast", "Remain" => "Calm"}
hsh ["Never"] = "Forget your towel"

# How would you perform an operation on every element inside a Hash?

I made this to spit out "{KEY} is {VALUE}"

beerhsh = {'Arrogant Bastard Ale'=>'Delicious', 'Anything by Rogue Brewery'=>'Exquisite', 'Old Rasputin'=>'Hearty', 
 'Heineken'=>'Donkey Urine'}
 beerhsh.each_pair do |key, val|
   puts "#{key} is #{val}"
end

# How would you change the value of a particular element in a Hash?

Using my above example, adding:

beerhsh['Old Rasputin'] = 'Un-kill-able'

# How do you delete an element from a Hash?

Using my above example, adding:

beerhsh.delete ('Arrogant Bastard Ale')

# What happens if you try to retrieve an element from a Hash that does not exist in the Hash?

We get a blank line and it returns nil.

# How do you determine how many elements are in a Hash?

puts beerhsh.length