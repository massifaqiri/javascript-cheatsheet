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
| Escape sequences | `\b`	Backspace <br /> `\f`	Form Feed <br /> `\n`	New Line |
