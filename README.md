<h2>Types, Values and Variables</h2>

Primitive types
Numbers
Strings
Booleans

Special JavaScript values
Null
Undefined

Object Type

Numbers

JS doesn't make a distinction between Integer and Floating-point values.
i.e. 1 and 1.0 are same numbers.
In JS all numbers are represented as floating-point values.
JS represents numbers using the 64-bit floating-point format.
Numeric literal
when a number appears directly in a JS program, it’s called a numeric literal.
Numeric literals can be preceded by a minus sign (-) to make the number negative. Technically, however, - is the unary negation operator and is not a part of the numeric literal.
Floating-point literals
2.36
	2563.4896
		JS Also supports Exponential notation
		6.02e23	// 6.02 * 1023	(base-10)
		6.02e-23	// 6.02 * 10-23	(base-10)
Integer literals
Base-10 integers
	9
	0
	897

Base-16 Hexadecimal values
			0xff	// 15*16 + 15 = 255 (base-10)
			0XCAfe546

Base-8 octal format
			0377	// 3*64 + 7*8 + 7 = 255 (base-10)
			Avoid using octal literal with leading 0, as all implementations of JS do not support octal literals. In ES5 strict mode, octal literals are explicitly forbidden.

Arithmetic in JS

Basic arithmetic operators
+ for addition
- for subtraction
* for multiplication
/ for division
% for modulo (remainder after division)

Complex arithmetic operations
	For complex operations JS provides a Math object which provides various methods to perform complex mathematical operations.

Overflow
It occurs when the result of a numeric operation is larger than the largest representable number.
The result is special infinity value, which JS prints as ‘Infinity’
For a negative number larger than the largest representable negative number JS prints ‘-Infinity’.
Infinity ( + or - or * or / or % ) any number = Infinity

Underflow
It occurs when the result of a numeric operation is closer to 0 than the smallest representable number.
In case of underflow JS returns 0
In case of underflow occurred from negative a number JS returns a special value ‘-0’ known as negative zero

Any number divided by 0 is not an error in JS, JS returns Infinity or -Infinity
In JS 0/0 evaluates to a special value NaN (not a number).
Infinity/Infinity => NaN
JS defines Infinity and NaN  as global variables.
In ES3 Infinity and NaN were read/write values but ES5 corrects it and made them read-only.

ToDo: Binary Floating-Point and Rounding Errors




Text

In JS a string is an immutable ordered sequence of 16-bit values, each of which typically represents a Unicode character.
Strings are JS type for representing text.
JS strings use zero-based indexing.


Boolean Values

A boolean value represents truth or falsehood, on or off, yes or no. there are only two possible values.
JS has two reserved keywords for boolean values, these are ‘true’ and ‘false’.


Null and Undefined


Null is a language keyword.
Null has a special value which indicates absence of a value.
Undefined is a predefined global variable (not a language keyword).
Undefined also indicates absence of value but in a deeper sense than Null.
Querying a variable, which is declared but not assigned with any value, returns ‘undefined’.
Querying value of a object-property or array-element which does not exist returns ‘undefined’.
Null == undefined evaluates to true indicating that both indicates absence of value.
Null === undefined evaluates to false indicating that both are of different type.
Null and undefined, both are falsy values.
Null and undefined, both have no properties or method, use of . or [] operator gives ‘TypeError’.
Undefined should be used to represent system-level, unexpected or error-like absence of value.
Null should be used to represent program-level, normal or expected absence of value.
If programmer needs to ( intentionally ) assign one of these values to a variable or property or pass one of these values to a function, Null is the right choice.





