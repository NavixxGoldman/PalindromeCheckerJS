# PalindromeCheckerJS
Return true if the given string is a palindrome. Otherwise, return false.  A palindrome is a word or sentence that's spelled the same way both forward and backward, ignoring punctuation, case, and spacing.
```javascript
function palindrome(str) {
  var newStr="";
  // Good luck!
  //Regex+toLowerCase
  var regex=/[\W_]/g; 
  var oldStr=str.replace(regex,"").toLowerCase();
  //reverse for palindrome
  newStr=str.replace(regex,"")
  .toLowerCase()
  .split("")
  .reverse()
  .join("");
  //Check for Palindrome
  if(oldStr==newStr){
     return true;
  }else{
    return false;
  }
 
}



console.log(palindrome("not a palindrome"));
console.log(palindrome("never odd or even"));
```
