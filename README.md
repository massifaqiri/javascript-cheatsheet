# Javascript Master Cheatsheet
| ???? | ?????? |
| --- | --- |
| Change HTML content | `document.getElementById("demo").innerHTML = "Hello World";` |
| Change HTML attribute value | `document.getElementById("MyImage").src = "AnotherImage.jpg"` |
| Change HTML style | `document.getElementById("demo").style.color = "red"` |
| Insert JS code in HTML using `<script>` | `<script> function changeColor() { ... } </script>` |
| Run an external function | `<script src="myFunction.js"></script>` <br /> 💡 You can use it inside head or body |
| Comment (one line) | `// This is a one line comment.` |
| Comment (multi line) | `/* This is a multi-line comment,` <br /> `that takes more than one line. */` |
| Declaring variable | `var` or `let` or `const` <br /> 💡 `let` and `const` are new ways of declaring variable and more preferable. `const` is commonly used for declaring constants. |
| Arithmetic operators | `+ (add),` <br /> `- (subtract),` <br /> `* (multiply),` <br /> `** (exponentiation),` <br /> `/ (division),` <br /> `% (modulus),` <br /> `++ (increment),` <br /> `-- (decrement)` |
| Assignment operators | `= (equal),` <br /> `+= (add up),` <br /> `-= (subtract),` <br /> `*= (multiply),` <br /> `/= (divide),` <br /> For example, `x += 2` is the same as `x = x + 2` |
| Comparison operators | `== (equal to),` <br /> `=== (equal value and equal type),` <br /> `!= (not equal),` <br /> `!== (not equal value or not equal type),` <br /> `> (greater than),` <br /> `< (less than)` <br /> `>= (greater than or equal to)` |
| Logical operators | `&& (and),` <br /> `\|\| (or),` <br /> `! (not),` |
| `typeof` | Returns the type of a variable |
| Bitwise operators | `& (AND), e.g., 0101 & 0001 = 0001` <br /> `\| (OR), e.g., 0101 \| 0001 = 0101` <br /> `~ (NOT), e.g., ~0101 = 1010` <br /> `^ (XOR), e.g., 0101 & 0001 = 0100` <br /> `<< (Left Shift), e.g., 0101 << 1 = 1010` <br /> `>> (Right Shift), e.g., 0101 >> 1 = 0010` <br /> 💡 Bit operators work on 32-bit signed numbers and it outputs decimal number (not bits) |
| Data types | 1. String, e.g. `let animal = "Cat";` <br /> 2. Number, e.g. const PI = 3.14;` <br /> 3. Booleans: `true` or `false` <br /> 4. Arrays, e.g. `let colors = ["red", "yellow"];` <br /> 5. Objects, e.g. `const topStudent = {firstName: "John", lastName: "Doe", age: 20};` <br /> 6. Undefined: a variable with undefined value has `undefined type` |
| Function | `function getSquare(num) {` <br /> &nbsp;&nbsp;&nbsp;&nbsp;`return num ** 2` <br />  `}` |
| Access object properties | `const name = topStudent.firstName;` assuming `const topStudent = {firstName: "John", lastName: "Doe", age: 20};` |
| Object methods | Object method is simply a function being the value of an object key, e.g. `const topStudent = {firstName: "John", lastName: "Doe", fullName: function() { return this.firstName + " " + this.lastName; } };` |
| `this` refers to ... | Object (inside an object), Global Object (alone and in a function), Element receiving the event (in an event) <br /> 💡 You can use `bind()`, `call()`, and `apply()` to refer `this` to any object |
| Escape character | `\`, e.g. `\"` will give `"` |
| Escape sequences | `\b`	Backspace <br /> `\n`	New Line |
| String length | `myString.length` assuming `myString = "ABCDE";` |
| Extract a part of a String | `myString.slice(1, 4)` as in `(start, end)`<br /> `myString.substring(1, 4)` as in `(start, end)` <br /> `myString.substr(1, 3)` as in `(start, length)`<br /> 💡 The end position is not included in both `slice` and `substring`. If you don't state the end position, both methods will extract the rest of the string from the start position. Only `slice` can work with negative numbers. |
| Replace String content | Replace the first occurrence:  `let newString = myString.replace("CurrentText", "NewText");` <br /> Replace all occurences: `let newString = myString.replace(/CurrentText/g, "NewText");` |
| Convert String to uppercase or lowercase | `let newString = myString.toUpperCase();` <br /> `let newString = myString.toLowerCase();` |
| Concatenate two or more strings | `let newString = myString.concat("some more text", " and even more text.");` |
| Remove whitespace from both ends | `let newString = myString.trim();` |
| Add padding at the beginning or end | `let paddedString = myString.padStart(4, "x");     // gives xxx2 assuming myString = "2"` <br /> `let paddedString = myString.padEnd(4, "x");     // gives 2xxx assuming myString = "2"` |
| Get character at desired position (index) | `myString.charAt(3);` |
| Get ASCII code of a character | `myString.charCodeAt(0);` |
| Split a String into array | Split on a delimiter: `myString.split(",");` <br /> Split all characters: `myString.split("");` |
| Get index of a desired character or substring | `myString.indexOf("book");` OR `myString.lastIndexOf("book");` <br /> 💡 You can specify a second parameter to state the start position of the search like, `myString.indexOf("book", 5); // starts the search at 5` |
| Search String | `myString.search("book"); // returns the position` <br /> `myString.match(/book/g); // takes regex and returns the matches as array` <br /> `myString.includes("book"); // returns true or false` <br /> 💡 Both `search` and `match` can search against regex. |
| `startsWith` and `endsWith` | Returns true or false if a string starts or ends with the given string. <br /> 💡 You can specify position (as optional param) for `startsWith` and length (as optional param) for `endsWith`. |
| Template Literals | `let title = 'World!';` <br /> \`Hello ${title}\`; |
| Scientific Notation of numbers | `let x = 123e5;` OR `let y = 123e-5;` |
| `NaN` | Stands for Not a Number. For example, `let x = 100 / "Apple"; \\ gives NaN` |
| Convert a number to other bases | `num.toString(16); // Hexadecimal` <br /> `num.toString(8); // Octal` <br /> `num.toString(2); // Binary` |
| Comparing two JavaScript objects always returns ... | false |
| Number methods | `toString()`: Converts the number to string <br /> `toExponential(2)`: Rounds up the number to the given number and returns it in exponential notation <br /> `toFixed(2)`: Returns the number with the specified number of decimals <br /> `toPrecision(2)`: Returns the number with the specified length <br />  |
| Convert other variables to number | `Number()` or `parseInt()` or `parseFloat()` |
| Infinity | `Number.POSITIVE_INFINITY` or `Number.NEGATIVE_INFINITY` |
| Largest or Smallest number in JS | `Number.MAX_VALUE` or `Number.MIN_VALUE` |
| Get or Set from array by index | `let myFaveCor = cars[0];` <br /> `cars[0] = "BMW";` |
| Get array length | `myArray.length` |
| Convert array to string | `toString()`: Converts an array to a string of comma-separated array values <br /> `join(" * ")`: Converts an array to a string, separated by the specified operator | 
| Remove from array | `pop()`: Removes the last element from an array <br /> `shift()`: Removes the first array element <br /> `splice(desiredPosition, numberOfItemsToRemove)`: You can remove items using `splice`. |
| Add to array | `push("An Item")`: Adds a new element to the end of the array <br /> `unshift("New Item")`: Adds the given items to the beginning of the array <br /> `splice(desiredPosition, numberOfItemsToReplace, "The New Item1", "The New Item 2");`: Adds new items to the array at the specified position. | 
| Merge two or more arrays | `arrayA.concat(arrayB)`: Concatenates two arrays and returns the merged array. Nb. You can merge more than one arrays with this method. | | Extract from array | `slice(startingPosition, optionalEndingPosition)`: Extract a portion of the array with the given start and end. |
| Sort array | `myArray.sort();` <br /> 💡 JS sorts elements as strings. To sort numbers, you should use `compare`. See below. |
| `compare` | Sort array numbers in ASC or DESC: `myArray.sort((a, b) => a - b);` or `myArray.sort((a, b) => b - a);`. <br /> You can also sort array of objects using `compare`: `myArray.sort((a, b) => a.year - b.year);` |
| Search Array | `includes(item)`: Checks if the item is present in the array. <br /> `indexOf(item, startOptional)`: Returns the index of the given item in the array. <br /> `lastIndexOf(item, startOptional)`: Returns the index of the given item (from the end) in the array. <br /> `let first = myArray.find((itemValue, itemIndexOptional, arrayOptional) => {return itemValue > 18;})`: Returns the first item that passes the test (function). <br /> 💡 There is also `findIndex` that works just like the above `find` method, except it returns its index. |
| Reverse Array | `myArray.reverse();` |
| Get min or max of array numbers | `Math.min.apply(null, myArray);` or `Math.max.apply(null, myArray);` |
| Looping Array | `myArray.forEach((itemValue, itemIndexOptional, arrayOptional) => {return itemValue * 2;})`: Applies the callback function on each array item. <br /> `let newArray = myArray.map((itemValue, itemIndexOptional, arrayOptional) => {return itemValue * 2;})`: Applies the callback function on each array item and returns the new array. <br /> `let newArray = myArray.filter((itemValue, itemIndexOptional, arrayOptional) => {return itemValue < 18;})`: Filters the array based on the boolean function given. <br /> `let sum = myArray.reduce((total, itemValue, itemIndexOptional, arrayOptional) => {return total + itemValue;})`: Applies the callback function on each array item and returns (reduces) them to a single value. 💡 There is also `reduceRight()` that works from right to left.  | 
| `every` and `some` | `let over18 = myArray.every((itemValue, itemIndexOptional, arrayOptional) => {return itemValue > 18;})`: Checks if _all_ values pass the given test (function). <br /> `let over18 = myArray.some((itemValue, itemIndexOptional, arrayOptional) => {return itemValue > 18;})`: Checks if _some_ values pass the given test (function). |
| | |
| | |
| | |
| | |
| | |
| | |
| | |
| | |
| | |
| | |
| | |
| | |
| | |
| | |
| | |
| | |
| | |
| | |



