---
title: Hashes
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a Hash?

A Hash is a collection of data elements that are indexed by a key that is another data element.

# What are some examples of information that would be Hashes as opposed to some other data type?

A Hash would be used to organize data into pairs, such as names and addresses or cities and states.

# How are Hashes and Arrays similar? How are they different?

Both are collections of data elements, but Arrays are indexed by sequential integers, while Hashes are indexed by other data elements.

# How do you retrieve a particular value from a Hash?

By using the data element associated with that value as the index key.

# How do you add information to a Hash?

Hash[new_key] = new_value

# How would you perform an operation on every element inside a Hash?

By using the each or each_pair methods.

# How would you change the value of a particular element in a Hash?

Hash[key] = new_value

# How do you delete an element from a Hash?

Hash.delete(key)

# What happens if you try to retrieve an element from a Hash that does not exist in the Hash?

It returns 'nil'.

# How do you determine how many elements are in a Hash?

Hash.length