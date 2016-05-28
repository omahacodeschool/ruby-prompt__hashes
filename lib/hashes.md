---
title: Hashes
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a Hash?

A Hash is similar to an array, in that it indexes objects. However, instead of being indexed by integers (0, 1, 2...), Hashes can use any type of object, such as strings. Therefore, hashes can store more specific and complex data than an array.
Hashes are made up of keys and values and are defined by curly brackets {}. Each key and value make up one pair.

# What are some examples of information that would be Hashes as opposed to some other data type?

You could use Hashes to store information about movies.
Example : star_wars = {"director" => "George Lucas", "genre" => "Science Ficton", "year" => "1977"}
You could also use Hashes to keep track of how many plants you have in your garden.
Example: plants = {"tomato" => "6", "onion" => "4", "carrots" => "6"}

# How are Hashes and Arrays similar? How are they different?

Hashes are similar to Arrays because they both index objects in an organized manner.
Hashes are different from Arrays in that you can index objects by more than just integers, like strings or symbols. This allows Hashes to be more organized, and you are able to retrieve data without having to loop through the hash like you would an array.

# How do you retrieve a particular value from a Hash?

You retrieve a value from a Hash based on its specific key using brackets [].
Example: I have a Hash with memebers of the original line up of the Ramones. I can't remember who played the bass.
ramones = {"vocals" => "Joey", "guitar" => "Johnny", "bass" => "Dee Dee", "drums" => "Tommy"}
ramones["bass"]
=>"Dee Dee"

In this example, vocals, guitar, bass and drums are the keys, and Joey, Johnny, Dee Dee and Tommy are the values.

# How do you add information to a Hash?

In order to add new information to a Hash, you would use the bracket equals method.
Example: I am using a Hash to keep track of animals I have on my farm. I just got two donkeys, and I need to add it to my exisiting Hash.
animals = {"cows" => "9", "chickens" => "4", "goats" => "1"}
animals[donkeys] = 2
puts animals
animals={"cows" => "9", "chickens" => "4", "goats" => "1", "donkeys" => "2"}

# How would you perform an operation on every element inside a Hash?

Use an each loop to apply a change to all elements inside a Hash. This allows you to make changes to both the key and the value inside the Hash.

# How would you change the value of a particular element in a Hash?

In order to change the value of a Hash, use brackets.
Example:
meal={"main course" => "regular steak", "side dish" => "jelly beans"}
meal["main course"]="milk steak"
puts meal
{"main course"=>"milk steak", "side dish"=>"jelly beans"}

# How do you delete an element from a Hash?

To delete an element from a Hash, use the delete method.
hash_name.delete("key_name")


# What happens if you try to retrieve an element from a Hash that does not exist in the Hash?

You retrieve nil, or nothing.

# How do you determine how many elements are in a Hash?

To determine how may key-value pairs you have in a Hash, use the .length method.
Example:
animals={"cows" => "9", "chickens" => "4", "goats" => "1", "donkeys" => "2"}
puts animals.length
=> 4