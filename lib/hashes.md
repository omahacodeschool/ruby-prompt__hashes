---
title: Hashes
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a Hash?

A Hash is similar to an Array but allows us to organize multiple lists together.

# What are some examples of information that would be Hashes as opposed to some other data type?

If you were making an errand list or maybe a packing list for a family, it would make more sense to use a Hash rather than another data type. You would be able to make specific lists tied to each type of errand or items needed for each family member.

# How are Hashes and Arrays similar? How are they different?

Both Hashes and Arrays can contain multiple elements that make up lists of data. The elements in an Array are addressed by using the indexed position in the Array starting at 0. Hashes on the other hand have keys and values. By using a Hash you can make more complex lists of data instead of being limited to a single list when using an Array.

# How do you retrieve a particular value from a Hash?

Values within a Hash are retrieved by calling it's key. So to find the value of _seafood = {"Fish" => "Bass"}_ you would call the key using _seafood["Fish"]_. 

# How do you add information to a Hash?

You can add information to a Hash when initializing it. This is done by assigning the keys and values you want in your new Hash to the name of your Hash. Once you've initialized your Hash you can add more information by using the [ ] = method. The key you want to add goes inside of the brackets and the value assgined to that key comes after the = sign. 

# How would you perform an operation on every element inside a Hash?

Arrays and Hashes both have an .each method which iterates over each element inside of them running the block of code we send in. The .each method for Hashes take two arguments, a key and a value.

# How would you change the value of a particular element in a Hash?

To change the value of an element in a hash you would use the same [ ] = method to assign a new value to the key.

# How do you delete an element from a Hash?

You can delete an element from a Hash by using the .delete( ) method and putting in the key you want deleted in as the argument.

# What happens if you try to retrieve an element from a Hash that does not exist in the Hash?

Ruby returns nil if you try to retrieve an element from a Hash that does not exist.

# How do you determine how many elements are in a Hash?

Using the .length or .count methods on a Hash will return the number of keys and value sets. If you wanted to see all the keys in your Hash returned, you could use the .keys method. To return all the values within a Hash you can use the .values method on the Hash name.