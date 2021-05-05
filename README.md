# MorningMethods
Method morning challenge
let array = ['a','b','c','d']
let array2 = [1,2,3,4,5]
let array3 =['this','is','an','array']

// every
o(n)
// this method tests whether all elements in the array pass the test implemented by the  function provided/ Boolean

array.every(i.length = 1)
// true
array2.every(i < 10)
// true
array3.every(i.length >= 2)
//false


// filter
o(n)
//  filter() method creates a new array with all elements that pass the test implemented by the provided function.

array.filter(array => array.length < 6);

// log
array = [1,2,3,4,5] 
array.filter(i.length < 2)
// ['a','b','c','d']
array2.filter(i % 2)
// [3,5]
array3.filter(i.length = 2 )
// ['is','an']

// forEach
0(n)
// The forEach() method executes a provided function once for each array element.

array.forEach((console.log(i)))
// a
// b
// c
// d
array2.forEach(i + 1)
// 2,3,4,5,6
array3.forEach( (i.length <= 2) + 1)
// 'this' , 'is1' ,'an1', 'array'

// includes
o(n)
//determines whether an array includes a certain value among its entries, returning true or false as appropriate.

array.includes('c')
// true
array2.includes('A')
// false
array3.includes('an')
//true

// indexOf
0(n)
//  returns the first index at which a given element can be found in the array, or -1 if it is not present

array.indexOf('b')
// 1
array2.indexOf( 1 )
// 0
array3.indexOf('an')
// 2

// map
0(n)

// method creates a new array populated with the results of calling a provided function on every element in the calling array

array2.map(i => i * 2)
// [2,4,6,8,10]
array2.map(i => i + 10)
// [11,12,13,14,15]
array2.map(i => i - 5)
// [-4,-3,-2,-1,0]

// pop
O(n)
//  method removes the last element from an array and returns that element. This method changes the length of the array.

array.pop('5')
// a,b,c,d,5
array2.pop('A')
// 1,2,3,4,5,A
array3.pop('pop')
// 'this','is','an','array,pop

// push
O(n)
// method adds one or more elements to the end of an array and returns the new length of the array.

array.push('5')
// 5
array2.push('A')
// 6
array3.push('pop')
//5

// reduce
0(n)
// method executes a reducer function (that you provide) on each element of the array, resulting in a single output value

reducer = (i , output) => i + output
array2.reduce(reducer)
// 15
array2.reduce(reducer, 10)
// 25
array2.reduce(reducer, -5)
// 10

// shift
O(N)
// method removes the first element from an array and returns that removed element. This method changes the length of the array.

array.shift()
//b,c,d
array2.shift()
//2,3,4,5
array3.shift()
//'is','an','array'

// slice
O(N)
// method returns a shallow copy of a portion of an array into a new array object selected from start to end (end not included) where start and end represent the index of items in that array. The original array will not be modified

array.slice(2)
// c,d
array2.slice(4)
// 5
array3.slice(0)
// 'this','is','an','array'

// sort
0(n log(n))
//  method sorts the elements of an array in place and returns the sorted array. The default sort order is ascending, built upon converting the elements into strings, then comparing their sequences of UTF-16 code units values

array.sort()
// a,b,c,d
array2.sort()
// 1,2,3,4,5
array3.sort()
// ["an", "array", "is", "this"]

// unshift
O(N)
//  method adds one or more elements to the beginning of an array and returns the new length of the array.

array.unshift('5' , '3')
// 6
array2.unshift('A' , 'b')
// 7
array3.unshift('pop' , 'lock')
//6

//STRING METHODS

str = 'this is a string'
str2 = 'and this is another string'


// charAt o(n)
// method returns a new string consisting of the single UTF-16 code unit located at the specified offset into the string.

str.charAt(5)
// expected
'i'
str.charAt(8)
// expected
'a'
str.charAt(11)
// expected
't'

// charCodeAt O(n)
// method returns an integer between 0 and 65535 representing the UTF-16 code unit at the given index.


str.charCodeAt(5)
// expected
'105'
str.charCodeAt(8)
// expected
'97'
str.charCodeAt(11)
// expected
'116'

// concat O(n)
// concatenates the string arguments to the calling string and returns a new string.

return str.concat(' ',str2)
// 'this is a string and this is another string'
return str2.concat(' ',str)
// 'and this is another string this is a string'
str3 = str.concat(' ',str2)
return str3

'this is a string and this is another string'

// includes O(n)
// performs a case-sensitive search to determine whether one string may be found within another string, returning true or false as appropriate.

str.includes('a')
// true
str2.includes('another')
// true
str.includes('another')
// false


// indexOf O(n)
// returns the index within the calling String object of the first occurrence of the specified value, starting the search at fromIndex. Returns -1 if the value is not found.


str.indexOf('a')
// 8
str2.indexOf('another')
// 13
str.indexOf('this')
// 0

// match O(n)
// retrieves the result of matching a string against a regular expression.

str.match()
// ['']
str.match(/[A-Z]/g)
// ['']
str2.match(/[abc]/g)
// ['a','a']



// repeat
// method constructs and returns a new string which contains the specified number of copies of the string on which it was called, concatenated together.

str.repeat(2)
// 'this is a string this is a string'
str.repeat(5)
// 'this is a string this is a string this is a string this is a string this is a string'
str2.repeat(3)
// 'and this is another string and this is another string and this is another string'

// replace O(n)
// method returns a new string with some or all matches of a pattern replaced by a replacement. The pattern can be a string or a RegExp, and the replacement can be a string or a function to be called for each match. If pattern is a string, only the first occurrence will be replaced.

str.replace('this','str' )
str.replace('string', 'sentence')
str2.replace('another', ' ')

// search O(n)
// executes a search for a match between a regular expression and this String object.

str.search(/[A-Z]/g)
// [-1]
str.search()
// []
str2.search(/[abc]/g)
// [0 , 12]


// slice O(n)
//  method extracts a section of a string and returns it as a new string, without modifying the original string

str.slice(13)
// 'ing'
str.slice(2,10)
// is is a s
str2.slice(5)
// his is another string

// split o(n)
// method divides a String into an ordered list of substrings, puts these substrings into an array, and returns the array.  The division is done by searching for a pattern; where the pattern is provided as the first parameter in the method's call.

str.split('')
// 't,h,i,s,i,s,a,s,t,r,i,n,g'
str.split(' ')
// 'this','is','a','string'
str2.split()
// and this is another string

// substr O(n)
// method returns a portion of the string, starting at the specified index and extending for a given number of characters afterwards.
substr(start, length)
str.substr(2,10)
str2.substr(2,10)

// toLowerCase O(n)
// method returns the calling string value converted to lower case.

str.toLowerCase()
// this is a string
str2.toLowerCase()
// and this is another string

// toUpperCase O(n)
// method returns the calling string value converted to upper case.
 str.toUpperCase()
// THIS IS A STRING
 str2.toUpperCase()
// AND THIS IS ANOTHER STRING

// trim O(log n)
//  method removes whitespace from both ends of a string.
string = '   this is a string to test trim   '
console.log(string.trim())
// 'this is a string to test trim'
string2 = 'this is another string   to  test trim'
console.log(string2.trim())
// 'this is another string to test trim'

string3 = 'this  is the last string ....  maybe.'
console.log(string3.trim())
// 'this is the last string... maybe.'

