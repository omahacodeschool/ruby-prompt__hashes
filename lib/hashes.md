---
title: Hashes
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a Hash?
A Hash is a unordered collection of data where each element is addressed by a name.
A Hash is a dictionary-like collection of unique keys and their values.
Hashes are also known as 'associative Arrays'.


# What are some examples of information that would be Hashes as opposed to some other data type?
Some examples of information that would be Hashes would be an unordered collection where data is organized into 'key/value' pairs. 
We can use Hashes when we want collect data such as 'refridgerator_items/number_each_item_left', or 'restaurant_menu/menu_item_price'. 


# How are Hashes and Arrays similar? How are they different?
Like Arrays, Hashes are collections of data.  Another way of thinking about how Hashes and Arrays are similar is both "have a bunch of slots that can point to various objects." -- Chris Pine, Learn to Program pg 115
Hashes and Arrays differ in that Hashes store data in keys and access that data by naming the key whose value we want to retrieve, while Arrays store data in numbered indexes and access that data via the index numbers.  Thus with Hashes we can use a key only once.


# How do you retrieve a particular value from a Hash?
We can retrieve particular values from a Hash using the '[]" operartor.
For example we'll start with a hash:   
    menu = {"Ramen"=>3, "Dal Makhani"=>4, "Tea"=>2}
We retrieve the value for "Ramen":
    menu["Ramen"] => 3


# How do you add information to a Hash?
We can add information to a Hash by using the '[] =' method.
For example:   
    menu = {"Ramen"=>3, "Dal Makhani"=>4, "Tea"=>2}
We'll add the line:  
    menu["Lobster"] = 25
The result: 
    menu => {"Ramen"=>3, "Dal Makhani"=>4, "Tea"=>2, "Lobster"=>25}


# How would you perform an operation on every element inside a Hash?
A way to perform an operation on every element inside a Hash is to use the '.each' method.
For example:  
    menu = {"Ramen"=>3, "Dal Makhani"=>4, "Tea"=>2, "Lobster"=>25}
We now want to lower prices by 25%
We add the following:  
    menu.each do |item,price|
        menu[item] = price + (price * -0.25)
    end
The result:
    menu => {"Ramen"=>2.25, "Dal Makhani"=>3.0, "Tea"=>1.5, "Lobster"=>18.75}


# How would you change the value of a particular element in a Hash?
Since with Hashes we can use a key only once, we can use the '[]=' method to overwrite a key/value pair.
For example back to our Hash:
    menu = {"Ramen"=>3, "Dal Makhani"=>4, "Tea"=>2, "Lobster"=>25}
We want to change Ramen to 5:
    menu[Ramen] = 5
The result:
    menu => {"Ramen"=>5, "Dal Makhani"=>4, "Tea"=>2, "Lobster"=>25}


# How do you delete an element from a Hash?
To delete an element from a Hash we can use the '.delete(key)' method.
For example back to our Hash:
    menu = {"Ramen"=>3, "Dal Makhani"=>4.5, "Tea"=>2, "Lobster"=>25}
We want to delete "Tea":
    menu.delete("Tea")
The result:
    menu => {"Ramen"=>3, "Dal Makhani"=>4.5, "Lobster"=>25}


# What happens if you try to retrieve an element from a Hash that does not exist in the Hash?
If we try to retrieve an element from a Hash that does not exist in the Hash we return => nil.
This is Ruby telling us the element we tried to retrieve does not exist.
In our example Hash:
    menu = {"Ramen"=>3, "Dal Makhani"=>4, "Tea"=>2, "Lobster"=>25}
We try to retrieve "Tofu":
    menu["Tofu"] => nil


# How do you determine how many elements are in a Hash?
Like with Arrays, we can use the '.count' method or '.length' method to determine how many elements are in a Hash.
We can also use the '.size' method.
In our example Hash:
    menu = {"Ramen"=>3, "Dal Makhani"=>4.5, "Tea"=>2, "Lobster"=>25}
Running the following methods:
    menu.count => 4
    menu.length => 4
    menu.size => 4
    