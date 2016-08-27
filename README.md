# Write a function that takes a string as input and returns the string reversed.


1. Reverse a String With Recursion

function reverseString(str) {
  return (str === '') ? '' : reverseString(str.substr(1)) + str.charAt(0);
}

comments: The depth of the recursion is equal to the length of the String. This solution is not the best one and will be really slow if the String is very long


2. Reverse a String with a for loop 
  
  var reverseString = function(s) {
    var result = "";
    for(var i = s.length-1; i >= 0; i--){
        result += s[i]; 
    }
    return result;
  };

3. You can also create a copy of the string into an array using the explode() method, then reverse the array using the reverse() method and finally changing the array back into a string using the join() method.
