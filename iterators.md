##Descriptions of Iterators

###Instructions
Below you will find a list of methods. In the space provided below each, please provide a brief description of what this method does based upon your review of the Docs. 

###Array methods:
May be helpful to look in [Enumerable](http://ruby-doc.org/core-2.2.0/Enumerable.html) as well...

####select: Assesses each element in an array with a provided block of code, and returns a new array populated with elements that return true for that given block. 

####reject: Like select, assesses each element in an array with a provided code, but returns a new array for which the element proves not true. 

####map: An alias for map is collect. Map and alias take a block of code and perform it on each element of the array. A new array is then returned, which is populated with the initial array's elements after having the block executed on them. 

####detect: An alias for detect is find. Find and detect return that first element in an array that proves true for a given block of code. 

####inject: An alias for inject is reduce. Reduce and inject are accumulating methods; they execute a binary operation to two elements, and the result is stored and used as the first of the two elements in the next comparison, thus accumulating. This binary operation can either be in block or symbol form. 

####partition: Partition is like a blend of select and reject. It executes a block of code on each element, placing the elements that return try in one array, and those that don't in another. Thus, partition returns two arrays. The first array is populated by the truthy elements, the second: falsey (is that a word ??)

####sort: Sorts the elements of an array dependent upon what the elements are, and a comparison that returns either -1, 0, or 1. This comparison is alphabetic for strings, and numeric for integers/floats. The comparison can be specified by a block of code.

####one: Called with .one?. Passes each element of the array to a block of code, returning true if EXACTLY ONE element of the array returns true from the block. Else: false as fuck. 

####none: Called with .none?. Passes each element of the array to a block of code, returning true if NONE of the elements return true for the block. Else, returns false.

####all: Called with .all?. Passes each element of the arry to a block of code, returning true only if every element returns true. Else, returns false. 

####empty?: Returns true if the receiver is empty. False otherwise. 

####eql?: Takes an array as a parameter. Returns true if the receiver array and parameter array both have the same content. 

####include?: Takes an object as a parameter. Returns true if the receiving array contains the given object parameter. Else: hella false. 

####nil?: Checks to see if a given object == nil. Returns true if that shit is nil, false if it aint.

###Hash methods:

####key?: Takes a key as a parameter, then checks to see if that key is present in the receiving hash. 

####keys: Returns a new array that is populated with a list of all the keys in the receiving hash. 

####delete: Takes a key as a parameter. Deletes a key-value pair, and returns the value of the pair that was deleted. If no matching key exists in the receiving hash, returns the default value, often nil. It is possible to specify a block of code, and the unfound key will instead return the result of the code block. 

####delete_if: Comparable to delete. However, rather than deleting a single key-value pair, instead deletes all key-value pairs for which a given block of code is true. Returns the hash, with remaining key-value pairs; i.e. those that evaluated to false. 
