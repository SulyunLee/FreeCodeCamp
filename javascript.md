<h1>JavaScript</h1>
* Comment<br>
```
// This is Comment
/* This is also comment */
```
* Create variable<br>
```
var ourname = "First var";
```

* ```.length``` property:<br>
Tell you how many characters are in the string.<br>

* Array declaration<br>
**Example**)<br>
```
var sandwitch = ["peanut butter", "jelly", "bread"];
```

* Access array data with indexes<br>
**Example**)<br>
```
var array = [1, 2, 3];
array[0];  // equals 1
var data = array[1];
```

* Variables which are defined outside of a function block have global scope.<br>
Variables which are used without the ```var``` keyword are automatically created in the global scope.

* ```.pop()``` function:<br>
Pop a value off of the end of an array. Any type of data structure can be popped off of an array - numbers, strings, even nested arrays.

* ```.push()``` function:<br>
Push data onto the end of an array.

* ```.shift()``` function:<br>
Remove the first element instead of the last.

* ```unshift()``` function:<br>
Add the element at the beginning of the array.

* Functions<br>
**Example**)<br>
```
function functionName(a, b){
  return a + b;
}
```

* Object:<br>
Similar to arrays but instead of using indexes to access and modify their data, you access the data in objects through 'properties'.<br>
**Example**)<br>
```
var cat = {
  "name": "Whiskers",
  "legs": 4,
  "tails":1,
  "enemies":["Water", "Dogs"]
};
```

* Update properties of object<br>
**Example**) Update name to "Happy Camper"<br>
```
cat.name = "Happy Camper";
```

* Delete properties from objects<br>
**Example**)
```
delete cat.tails;
```

* Random number generator<br>
<code> Math.random() </code> : Generate a random decimal.<br>
<code> Math.floor() </code> : Round the number down to its nearest whole number.<br>
**Example**) Generate between 0 and 19<br>
```
Math.floor(Math.ranadom() * 20);
```

* Regular expressions:<br>
Use to find certain words or patterns inside off strings<br>
**Example**) Find the word 'the' in the string<br>
```
/the/gi   // g means that we want to search the entire string
          // i means that we want to ignore the case when searching
```

* Digit selector:<br>
Used to retrieve the numbers in a string<br>
```
/\d/g
```

* Whitespace selector:<br>
```
/\s/g
```
**Match anything that isn't whitespace**<br>
```
/\S/g
```

* Create objects using constructor functions<br>
```
var MotorBike = function(){
  this.wheels = 2;
  this.engines = 1;
  this.seats = 2;
}
```

* Test objects for properties<br>
<code>.hasOwnProperty([propname]) method</code>
Return ```true``` or ```false``` if the property is found or not.<br>
**Example**)
```
var myObj = {
  top:"hat",
  bottom: "pants"
};
myObj.hasOwnProperty("top");  // true
myOjb.hasOwnProperty("middle");  // false
```

* JavaScript object notation JSON<br>
Use format of JavaScript objects to store data. JSON is flexible because it allows for Data Structures with arbitrary combinations of strings, numbers, booleans, arrays, and objects<br>
JSON objects can contain both nested objects and nested arrays.<br>
**Example**)<br>
```
var ourMusic = [
  {
    "artist":"Daft Punk",
    "title":"Homework",
    "release_year":1997,
    "formats":[
      "CD",
      "Cassette",
      "LP"
    ],
    "gold":true
  }
];
```

* ```map``` method:<br>
Iterate through arrays.<br>
**Example**) Iterate through every element of the array, creating a new array with values that have been modified by the callback function and return it.<br>
```
var timesFour =
oldArray.map(function(val)){
  return val * 4;
}
```

* ```reduce``` method:<br>
Iterate through an array and condense it into one value.<br>
To use reduce, you pass in a callback whose arguments are an accumulator(```previousVal```) and the current value(```currentVal```).<br>
Optional second argument: used to set the initial value of the accumulator.<br>
**Example**) Sum all the values in array and assign it to <code>singleVal</code>.<br>
```
var singleVal = array.reduce(function(previousVal, currentVal){
  return previousVal + currentVal;
});
```

* ```filter``` method:<br>
Iterate through an array and filter out elements where a given condition is not true.<br>
filter is passed a callback function which takes the current value as an argument(```val```).<br>
**Example**) Remove array elements that are equal to five.<br>
```
array = array.filter(function(val){
  return val !== 5;
});
```

* ```sort``` method:<br>
Easily sort the values in an array alphabetically or numerically.<br>
Actually alters the array in place.<br>
**Example**) Sort the elements from smallest to largest number<br>
```
var array = [1, 12, 21, 2];
array.sort(function(a, b){
  return a - b;
  })
```

* ```reverse``` method:<br>
Reverse the elements of an array.<br>

* ```concat``` method:<br>
Merge the contents of two arrays into one.<br>
**Example**)<br>
```
newArray = oldArray.concat(otherArray);
```

* ```split``` method:<br>
Split a string into an array.<br>
Use the argument you pass in as a delimiter to determine which points the string should be split at.<br>
**Example**)<br>
```
var array = string.split('s');
```

* ```join``` method:<br>
Join each element of an array into a string separated by whatever delimiter you provide as an argument.<br>
**Example**)<br>
```
var joinMe = ["Na", "Na", "Na", "Na", "Batman!"];
var joinedString = joinMe.join("Na ");
```
