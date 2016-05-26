---
title: Hashes
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a Hash?

A hash is a collection of elements that are stored according to a key object.

# What are some examples of information that would be Hashes as opposed to some other data type?

A dictionary is one good example: each key word would be associated with a definition.  A hash could also be used to associate a list of books with their authors, with the title strings as the keys.  This would allow easily retrieving the author of a given book, or the definition of a given word.

# How are Hashes and Arrays similar? How are they different?

Both are lists of elements.  Arrays are ordered and each element has a numerical index.  Hashes instead have keys.  This makes it easier to look up the data associated with the key without having to do matching first to find the approriate index.

# How do you retrieve a particular value from a Hash?

Using square brackets, much as with an array, but instead of having the integer index, you would use the key object, such as:  hash["key"]

# How do you add information to a Hash?

During creation, you can add key-value pairs inside the braces.  After creation, you'd reference the key, even if it doesn't already exist, the same way you would to retrieve a value, with brackets.

# How would you perform an operation on every element inside a Hash?

Hashes have the each method the same way that arrays do.

# How would you change the value of a particular element in a Hash?

Using the bracket notation above, you would do: hash["key"] = new_value

# How do you delete an element from a Hash?

You would use the delete method on the hash, with the key of that element as the input.

# What happens if you try to retrieve an element from a Hash that does not exist in the Hash?

It will return nil.

# How do you determine how many elements are in a Hash?

Using the length method on the hash.