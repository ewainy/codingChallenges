**Given an integer x, return true if x is a palindrome, and false otherwise.**

 

Example 1:

``` 
Input: x = 121
Output: true
Explanation: 121 reads as 121 from left to right and from right to left.
```

Example 2:

```
Input: x = -121
Output: false
Explanation: From left to right, it reads -121. From right to left, it becomes 121-. Therefore it is not a palindrome.
```

Example 3:

```
Input: x = 10
Output: false
Explanation: Reads 01 from right to left. Therefore it is not a palindrome.
```

## My Solutions
Palindromes read the same left or right. 
Knowing that arrays have a reverse function... I wanted to:
- Convert the number to a string
- Use the split method to convert the string into an array of characters
- Use the reverse method to reverse the order
- Use join to reassemble the reversed characters into a string
- Check that the string and reverse string equal, if so, return true
- Otherwise return false


``` ts 
function isPalindrome(x: number): boolean {

const str = x.toString()
const reverse = str.split('').reverse().join('')

if (str === reverse) {
    return true
}

else {
    return false
}
    
};

```

``` ts

// using the String() constructor
function isPalindrome(x: number): boolean {

const str = String(x)
const reverse = String(x).split('').reverse().join("")


if (str === reverse) {
    return true;
} 

else {
  return false
}
    
};
```
