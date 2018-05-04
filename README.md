# Binary-search
# Using binary search to sort data 
# In lecture we discussed the binary search algorithm which searches a sorted array for a key and returns either the index of where it was found, or if not found, returns the index of where it belongs. In such a case this belongs index is encoded as a negative number to distinguish it from being confused with a found index. The encoding is as follows: add 1 to index then negate. In lecture we also discussed the insertInOrder algorithm which reads a sequence of values from a source ( text file) and inserts them into an array keeping them sorted as each value is added to the array. For this project you will get your input from a random number generator. YOu will use your bSearch to determine where that number belongs in the array, then the insertInOrder code will write a loop to open up a slot for that element and put the value into the array. THe call to bSearch will figure out where the new key belongs in O(Log2N), where as a linear scan will take O(N). Using a binary search instead of a simple linear scan to figure out where the new key goes is an optimization of the insertInOrder algorithm. When the insertInOrder gets the index back from the binary search, it must examine that value to see if it is negative. If so, it must be decoded back to a real index. The decoding is actually the same operation: add one then negate it (back to positive).
UPDATE
