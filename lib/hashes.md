---
title: Hashes
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a Hash?

    # A hash is a list of keys and values that are associated to eachother. You 
    # use curly brackets ({ }) at the beginning and ending of a hash. Hashes are not
    # ordered, so the last key-value pair added may not appear last when iterating
    # through that hash.

# What are some examples of information that would be Hashes as opposed to some other data type?

    # email => password
    # name => address/phone number
    # student => grade
    

# How are Hashes and Arrays similar? How are they different?

    # Similar: Both are lists of information that can be retrieved later,
                both can be iterated through, can add elements to both after they 
                are created
    
    # Different: Arrays are ordered, while hashes are not. Hashes contain key
            value pairs. You can use index to look up elements in an array, but 
            have to use the keys to look up values in a hash. Keys in a hash must 
            be unique, but elements in an array may be repeated.

# How do you retrieve a particular value from a Hash?

    # You can use the key to retrieve a particular value from a hash: hash_name[key]
    # This method will retrun the value of a particular key

# How do you add information to a Hash?

    # hash_name[key] = value... this will add the key:value pair to the hash

# How would you perform an operation on every element inside a Hash?

    # You can use the each method, each_value method or each_key method. 
    # each can perform an operation on all of the keys and vaulues within a hash
    # each_value will perform the operation on all of the values while each_key
    # will perform an operation on all of the keys.

# How would you change the value of a particular element in a Hash?

    # hash[key] = new_value, it is the same process as adding a new key:value pair,
    # since you can't have the same key appear more than once in a single hash.

# How do you delete an element from a Hash?

    # To delete an element from a hash you can use the delete method: hash.delete(key)
    # Both the key and value are removed from the hash.

# What happens if you try to retrieve an element from a Hash that does not exist in the Hash?

    # It won't cause an error, but it won't output anything

# How do you determine how many elements are in a Hash?

    # The length method will return how many key-value pairs are in a hash
    # hash.length