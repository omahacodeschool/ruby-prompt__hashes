---
title: Hashes
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

#THE NEW STUFF IS UP HERE AT THE TOP NOW. THESE TWO LITTLE PROGRAMS.

# How would you perform an operation on every element inside a Hash?

#TO PERFORM AN OPERATION ON EVERY ELEMENT IN A HASH -- NEW AND IMPROVED! My operation was to put each key-value pair in a sentence.
StateCaps2 = Hash.new{}
StateCaps2 = {"Idaho"=>"Boise", "Oregon"=>"Salem", "Vermont"=>"Montpelier", "Iowa"=>"Des Moines"}
StateCaps2.each {|key, value| puts "The capital of #{key} is #{value}."}


# How would you change the value of a particular element in a Hash?


#TO CHANGE ONE ITEM IN A HASH -- NEW AND IMPROVED! NO MORE MERGE! I learned about the rehash method, which will update the 
#hash with any changed values. In this case, I changed the capital of Oregon from Portland to Salem. In repl.it, this returned
#the entire "statecaps" hash with "Salem" where "Portland" was. 
statecaps = Hash.new{}
statecaps = {"Idaho"=>"Boise", "Oregon"=>"Portland", "Vermont"=>"Montpelier", "Iowa"=>"Des Moines"}
statecaps["Oregon"] = "Salem"
statecaps.rehash





# What is a Hash?

A hash is like an array except that you can use anything, not just a number, as the index. A hash associates one thing with
another thing, no matter what the two things are. Several of the sources I was looking at referred to a hash as a collection of 
"key-value pairs" so I dug around for a description of a key-value pair that made sense to me. The one I found described the "key" 
as the name of a container and the "value" as the contents of the container. The key 
does not have to be a number. The key can be a number, or a letter, or a string, or any other object that Ruby has available.
Because the variables in a hash are not indexed by number, there is no "first" one, "second" one, etc. To associate 
items in a hash, use a "rocket" which is this: =>.

# What are some examples of information that would be Hashes as opposed to some other data type?

Anything where you have to associate 2 ruby objects: A name and an email address, a menu item and a price, a novel
and an author, etc. 

# How are Hashes and Arrays similar? How are they different?

Hashes and Arrays are similar in that they are both collections of variables. Neither an Array nor a Hash has to be all numbers,
or all strings, or all floats, etc., all can be combinations of different types of variables. They are different in that Arrays
have an enumerated order to them and Hashes do not. To go back to the description of a key-value pair I used in the "What is a Hash" question
with an Array the name of the container (the key) would always be a number, and the value could be a variety of things. With a Hash
the name of the container could be any Ruby object.

# How do you retrieve a particular value from a Hash?

Retrieve a particular value by using its key. After many failures I did this with a simple hash in repl.it.
#NOTE I am including all of these bits of code that I try in repl.it because I am saving these as notes pages, and
I want to include the code in my notes pages. I am not trying to see how much code I can turn in or anything like that.
I know you aren't looking for code.

StateCaps2 = Hash.new{}
StateCaps2 = {"Idaho"=>"Boise", "Oregon"=>"Salem", "Vermont"=>"Montpelier", "Iowa"=>"Des Moines"}
puts StateCaps2.keys.inspect
puts StateCaps2.values.inspect
puts StateCaps2["Vermont"] #This returns just the capital of Vermont, which is "Montpelier.


# How do you add information to a Hash?

There are probably several ways to do this, but I found a Merge method that works kind of like "join".
I made a second hash of more states and capitals, then used the merge! method to make one larger hash.
This tacked on the new variables at visually at least is the "end" of the old hash.
StateCaps2 = Hash.new{}
StateCaps2 = {"Idaho"=>"Boise", "Oregon"=>"Salem", "Vermont"=>"Montpelier", "Iowa"=>"Des Moines"}
StateCaps3 = {"New York"=>"Albany", "Texas"=>"Austin", "Kentucky"=>"Frankfort"}
StateCaps2.merge! StateCaps3
puts StateCaps2

# How would you perform an operation on every element inside a Hash?

This seems like something that calls for a loop, specifically an "each do end" loop.
The bit of code below is an adaptation of found material, which isn't my favorite way to do this, 
and I'm still working backwards a little bit to say what everything does. Mostly I am taking out
pieces that I don't understand and seeing what error message I get. I get the impression that 
the "#" before {key} and {value} tells Ruby to evaluate each key and value in the hash and loop them into the appropriate places
one at a time. The block | | thing is starting to make sense. Need to do a lot more coding before any of it is like English.

StateCaps2 = Hash.new{}
StateCaps2 = {"Idaho"=>"Boise", "Oregon"=>"Salem", "Vermont"=>"Montpelier", "Iowa"=>"Des Moines", "New York"=>"Albany", "Texas"=>"Austin", "Kentucky"=>"Frankfort"}
StateCaps2.each do 
    |key, value| puts "The capital of #{key} is #{value}."
end



# How would you change the value of a particular element in a Hash?
There is probably a much more elegant way to do this than what I have done here. Using the states and capitals hash again, I changed
the capital of Oregon from Salem to Portland. It's not right, but let's say it is. It looks like the merge found the 
key "Oregon" and over-wrote the old capital "Salem" with the new one, "Portland." There is probably a way to do this
in one line of code.



PROGRAM TO CHANGE THE VALUE OF AN ELEMENT IN A HASH. let's say Oregon moved its capital to Portland and we had to update records.
StateCaps2 = Hash.new{}
StateCaps2 = {"Idaho"=>"Boise", "Oregon"=>"Salem", "Vermont"=>"Montpelier", "Iowa"=>"Des Moines", "New York"=>"Albany", "Texas"=>"Austin", "Kentucky"=>"Frankfort"}
StateCaps3 = {"Oregon"=>"Portland"}
StateCaps2.merge!(StateCaps3) 
puts StateCaps2["Oregon"] #NOTE the output for this is Portland

# How do you delete an element from a Hash?

I found 2 ways to delete an element and used both. The "Shift" method deletes the first key-value pair in the hash. The "Delete" method
allows you to specify which key-value pair you want to delete. You have to include the key with the method.
StateCaps2.delete "Vermont" removes "Vermont=>"Montpelier. StateCops2.shift removed "Idaho"=>"Boise".
So even though the key is not a number, Ruby makes some kind of determination about what to delete 
when you use "Shift."

# What happens if you try to retrieve an element from a Hash that does not exist in the Hash?

Who knows if this is an adequate test, but using my state and capitals hash, I tried to retrieve the capital of 
Nebraska, which isn't in the hash, along with a few values that could be retrieved. It left a blank line where 
that value would have gone if it had existed in the hash. 

# How do you determine how many elements are in a Hash?

The "size" method seems to work with hashes the same way the
"length" method works with arrays. In my test with my "StateCaps2" hash,
"The size of StateCaps2 is #{StateCaps2.size}" the size was 4. So it was counting each key-value pair as 1.