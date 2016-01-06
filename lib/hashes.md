---
title: Hashes
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a Hash?

A hash is a collection of data that includes unique keys and their corresponding values.

# What are some examples of information that would be Hashes as opposed to some other data type?

An examle of information that would use hashes would be team stats for a football team. Another example could be a restaurant menu that 
keeps track of the price or calories corresponding to each menu item.

# How are Hashes and Arrays similar? How are they different?

Arrays and Hashes are similar in that they can both contain a mixture of different kinds of data and values. What makes them different is that
Arrays use integers for indices and Hashes can use any object type. Also, a hash contains key and value pairs, whereas arrays can be any combination
of values.

# How do you retrieve a particular value from a Hash?

We can retrieve values from a hash using the "[]" operator. 
If the name of our hash is "my_car" and we wanted to find out its "top speed" (assuming such value was supplied), we could use "[]" as follows:
my_car["top speed"]

# How do you add information to a Hash?

Continuing the above example, if we wanted to add the color to my_car, we could do this by using the following code:
my_car["color"] = "blue"

# How would you perform an operation on every element inside a Hash?

You can use an "each" loop to iterate through a hash and manipulate its values. Say I have the following hash and I want to increase all of its values
by 25%. I can do this as follows:
my_car = {"top speed => 115, "odometer miles" => 25430, "number of cylinders" => 4}
my_car.each do |feature, stat|
my_car[feature] = stat + (stat * 0.25)
end

# How would you change the value of a particular element in a Hash?

Now, if I wanted to change only the "odometer miles" on my_car to 15,000, I could do this like so:
my_car["odometer miles"] = 15000

# How do you delete an element from a Hash?

We could delete an element (let's say "top speed" from our above example by using the "delete" method. This looks like:
my_car.delete("top speed")


# What happens if you try to retrieve an element from a Hash that does not exist in the Hash?

If you try to retreive an element that does not exist in the Hash, you get the following (we'll use "top speed" as an example, since we just deleted it):
=> nil

# How do you determine how many elements are in a Hash?

We can use the "length" method in a hash to retrieve the number of "key value pairs".
If we take the above Hash and use the length method, it looks like this:
my_car = {"top speed => 115, "odometer miles" => 25430, "number of cylinders" => 4}
my_car.length (this would give us => 3).