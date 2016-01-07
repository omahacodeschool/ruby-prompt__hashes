---
title: Hashes
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a Hash?

A hash is sort of like a dictionary. Arrays are just a numbered list of items, but a hash is a list of items and their associated values (like words in a dictionary PLUS their definitions) and those items are recalled according to their names or “keys,” instead of by what numbered position they are on a list.

# What are some examples of information that would be Hashes as opposed to some other data type?

Anything that doesn’t work as just a numbered list. A dictionary wouldn’t, of course, because you’re not going to remember that “oligarch” is the 23,485th entry in the dictionary, you’re just going to remember the word oligarch (the key) and retrieve the definition from there. Your example is helpful, too – making a list of things you need to buy is not useful if they’re coming from multiple stores, but putting them in a hash with each store as key works really well for organizing that kind of two-layered (I guess you could call it that?) data. Makes me wonder if there are further structures to use in Ruby that allow for more than two layers of data, or if we’ll learn how to further index layers within hashes, if that makes any sense (like if you’re going to break up your shopping list according to stores AND sections of each store). Exciting!

# How are Hashes and Arrays similar? How are they different?

They’re similar in that they can both hold lists of data, have elements assigned, added and removed in a similar fashion, but arrays are really one-dimensional in that all you can do is make a numbered list. Hashes are more dynamic because of, well… I guess basically what I said on the last answer. 

# How do you retrieve a particular value from a Hash?

You do that like you would with an array, but instead of putting an index number between the brackets you would put the key you want to retrieve the value for.

# How do you add information to a Hash?

To add data to a hash, you use the “bracket equals” method. I know you’re not asking for code (sorry!), but it looks like this:

Beatles = { "Paul" => "singer/bassist", "John" => "singer/guitarist", "George" => "lead guitarist" }
Beatles["Ringo"]= "drummer"
Beatles          # output is all the info in the newly updated hash

# How would you perform an operation on every element inside a Hash?

You can iterate over all the elements in a hash using the each method, similar to arrays but it can pass information on to both the key and the value.

# How would you change the value of a particular element in a Hash?

OK – I overlooked the same concept with arrays but I get it now. It works kinda the same way as assigning a key/value in the first place. You would just enter that information again and it basically overwrites what was there before, right? I can’t help myself – here’s more unsolicited code:

Beatles = { "Paul" => "the cute one", "John" => "singer/guitarist" }
Beatles["Paul"] = "singer/bassist"
Beatles          # output is complete hash with newly changed info

# How do you delete an element from a Hash?

To delete from a hash (let’s say it’s called “new_hash” and the keys are a, b, c, d, and so on), put new_hash.delete(“b”) or put whatever other key name in the parentheses that you want to delete. This removes both the key and the value.

# What happens if you try to retrieve an element from a Hash that does not exist in the Hash?

The default is for Ruby to return nil, but there’s a way to make it return an assigned message, too. 

# How do you determine how many elements are in a Hash?

If you enter your hash_name.length Ruby will tell you how many elements are in the hash.