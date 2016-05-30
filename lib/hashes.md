---
title: Hashes
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a Hash?

A hash is like an array and separates a group of values into a list, but unlike an array, hashes identify each element value by an associated key.



# What are some examples of information that would be Hashes as opposed to some other data type?

Inventory information would be useful to be stored as Hashes, such as produce items, or apparel.



# How are Hashes and Arrays similar? How are they different?

Similar to an array, a hash separates a group of values into a list, but different from an array, hashes identify each element value by an associated key and finds them using a key, rather than relying on a value's position in a list, like an array does.



# How do you retrieve a particular value from a Hash?

You retrieve a hash value by referencing the key you want to retrieve the value from:

1) parts = {"alternators" => 8, "starters" => 16, "mufflers" => 7, "brake rotors" => 22}
2) puts parts["alternators"]   
(Result)=> 8




# How do you add information to a Hash?

You can add information to a has by using the ".merge" method on an existing hash:

1) parts = {"alternators" => 8, "starters" => 16, "mufflers" => 7, "brake rotors" => 22}
    (Result) => {"alternators"=>8, "starters"=>16, "mufflers"=>7, "brake rotors"=>22}

2) parts.merge("spark plugs" => 38)
    (Result) => => {"alternators"=>8, "starters"=>16, "mufflers"=>7, "brake rotors"=>22, "spark plugs"=>38}


# How would you perform an operation on every element inside a Hash?

In the following example, I define a hash, add an additional element to the hash, then call each key/value combo to be used in a sentence:

1) parts2 = {"alternators" => 8, "starters" => 16, "mufflers" => 7, "brake rotors" => 22}
2) parts3 = parts2.merge("spark plugs" => 38)
3) parts3.each {|key, value| puts "There are #{value} #{key} in stock at the main store." }
(Result)    There are 8 alternators in stock at the main store.
            There are 16 starters in stock at the main store.
            There are 7 mufflers in stock at the main store.
            There are 22 brake rotors in stock at the main store.
            There are 38 spark plugs in stock at the main store.
            => {"alternators"=>8, "starters"=>16, "mufflers"=>7, "brake rotors"=>22, "spark plugs"=>38}


# How would you change the value of a particular element in a Hash?

Changing the value of a hash is accomplished by assigning a new value to a specific key:
1) parts = {"alternator" => 8, "starter" => 16, "muffler" => 7, "brake rotor" => 22}

2) puts parts   
(Result) => {"alternator"=>8, "starter"=>16, "muffler"=>7, "brake rotor"=>22}

3) parts["alternator"] = 34

4) puts parts 
(Result) => {"alternator"=>34, "starter"=>16, "muffler"=>7, "brake rotor"=>22}



# How do you delete an element from a Hash?

Deleting an element from a hash is accomplished using the following syntax:

1) parts = {"alternator" => 8, "starter" => 16, "muffler" => 7, "brake rotor" => 22}
2) parts.delete("alternator")
(Result) => 8



# What happens if you try to retrieve an element from a Hash that does not exist in the Hash?

It will return a nil value.



# How do you determine how many elements are in a Hash?

Similar to arrays, one can use the ".size" or ".length" methods to determine the number of elements in a hash:

parts = {"alternator" => 8, "starter" => 16, "muffler" => 7, "brake rotor" => 22}
parts.size  => 4