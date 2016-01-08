---
title: Hashes
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
# What is a Hash?

A hash is a list of things (keys) and data associated with those things (values).

(# What are some examples of information that would be Hashes as opposed to some other data type? & # How are Hashes and Arrays similar? How are they different?)

Hashes and arrays are both lists that store data, and one can perform functions to each of the items on the list. However, hashes allow you add specific values to the different items on the list (prices on menu items, ages of students, or various facts about a single user [age=25, height=6’4, etc]) They are also organized very differently. An array has numbered slots, so you have to remember the number of the slot in order to retrieve data, and new items are added to either the beginning or end of the array (and thus they get their own numbered slot). In a Hash, it’s more like…a pile. Things just get added to the pile, with no beginning and no end.

# How do you retrieve a particular value from a Hash?
To retrieve a value, you just need the name of the hash and the name of the key whose value you are trying to find. Example foods[:pizza] would return => “best”
(Shannon question: this doesn’t work the opposite way. How would I search for “best” on a hash of foods?)

(# How do you add information to a Hash? # How would you change the value of a particular element in a Hash? # How do you delete an element from a Hash? )

You can easily add new things to a hash by just telling ruby what the new key equals. To the above list, I can add foods[:nachos] = “second best” and it will add it to the pile. Since every key in the pile has a specific name, if you do that to a key that is ALREADY in the pile, it will change the value of a pre-existing hash: foods[:pizza] = “best EVER” (or changing the price on a menu, or increasing the grade of a student, etc) If you want to REMOVE items from a hash, you use .delete (if, say, you develop a tragic adult onset tomato allergy, and have to perform foods.delete(":pizza”), it will remove it from the list)

# How would you perform an operation on every element inside a Hash?

You can use .each/do to perform an operation on every elements. For the food list example:
 foods.each do | item, value |
  puts "#{item} = #{value}" + " but better with cheese"
end
And then you basically have a recipe book.

# What happens if you try to retrieve an element from a Hash that does not exist in the Hash?

If you try to retrieve an element that isn’t there, you get the answer of “nil” (meaning “there’s nothing by that name in the pile”) If you want there to be a specific response to nonexistent elements, you can assign a .default. For my previous example, you could assign foods.default = “we don’t care about that food” so when someone asks foods[:eggplant] they will get that as a response instead of “nil"

# How do you determine how many elements are in a Hash?
I’m not sure I have the most elegant answer to this question, but right now the way i would do it is by using .keys. Continuing this example, I could do foods.keys and it would return “pizza, nachos, french fries, toast” and then I could just count those.