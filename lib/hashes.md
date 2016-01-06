---
title: Hashes
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a Hash?

It's a place to store data. It's unordered and they use a key/value system instead of number index like arrays. The key must be unique for each hash

# What are some examples of information that would be Hashes as opposed to some other data type?

You could store the totals number of items a cat likes that another cat also likes. You would be referring to a different table with items that would be stored in a hash 

# How are Hashes and Arrays similar? How are they different?

They can both store may times of data (integers, floats, strings), but arrays are ordered and hashes are unordered. Hashes are better for easily referencing their values using the key.

# How do you retrieve a particular value from a Hash?
By references it's particular key

    clems_friends = Hash.new(0)
    clems_friends["Kitten"] = 8
    clems_friends["Gita"] = 6
    puts clems_friends["Kitten"]

(in repl.it I'm getting the follwing output for the above code and I'm not sure why:

    8
    => nil
    
   I gave the hash a default value (0) so why is it returning 'nil'?)
   
   
# How do you add information to a Hash?
By either creating a hash and it's beginning key/value pairs in one line:

    clems_friends = { "Kitten" => 8, "Gita" => 6 }
    
or by first creating a hash, and then adding key/value pairs later:

    clems_friends = Hash.new(0)
    clems_friends["Kitten"] = 8
    clems_friends["Gita"] = 6

# How would you perform an operation on every element inside a Hash?
Use .each. If you only want to return the either the key or the value, you have to use block parameters. 'friend' is used for the key and 'total' is used for the value.

    clems_friends = { "Kitten" => 8, "Gita" => 6 }
      clems_friends.each do |friend, total|
          puts friend
      end

# How would you change the value of a particular element in a Hash?
You could use the same syntax from when you created the key/value pair from above:

    clems_friends["Kitten"] = 10

# How do you delete an element from a Hash?
use the .delete function.

    clems_friends.delete("Gita")

# What happens if you try to retrieve an element from a Hash that does not exist in the Hash?

It depends on whether or not you assigned a default value to the hash. 
If you did, then your code will return the default value, otherwise it will just return 'nil'

# How do you determine how many elements are in a Hash?
Use the .count method. This was hard to find anywhere. 
Maybe I wasn't looking for the right thing but eventually I just gave up searching and tried making up a method and it worked.

    clems_friends.count
     => 2