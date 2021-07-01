# LearningJournal-09

Class 1/jul/2021 

## 7 Types of Native Errors in JavaScript You Should Know
![img](https://miro.medium.com/max/1400/1*6uikTirxl4OZoJ5Qlo2UPA.jpeg)

1. RangeError
This is thrown when a number is outside an allowable range of values.

2. ReferenceError
This error is thrown when a reference made to a variable/item is broken. That is the variable/item doesn’t exist.

3. SyntaxError
This is the most common error we encounter. This error occurs when we type code that the JS engine can understand.
This error is caught by the JS engine during parsing.
There are different stages in the JS engine our code is put through before we see those results on the terminal.
* tokenization
* parsing
* interpreting
tokenization breaks the source of the code into individual units. At this stage, numbers, keywords,
literals, operators are sorted out and individually marked.
Next, the token stream generated will be passed to the parsing stage, which is handled by a parser.
This is where an AST is generated from the token stream. AST is an abstract representation of the structure of our code.
During these two stages, tokenization and parsing, if the syntax/source of our codes doesn’t conform to the syntax rules of JS makes the stages fail and throw SyntaxError.

4. TypeError
TypeError is used to indicate an unsuccessful operation when none of the other NativeError objects are an appropriate indication of the failure cause.
TypeError occurs when an operation is performed on a wrong data type. Maybe a boolean is expected but a sting is found.

5. URIError
This indicates that one of the global URI handling functions was used in a way that is incompatible with its definition.
URI (Uniform Resource Indicator) in JS has the functions: decodeURI, decodeURIComponent, etc.

6. EvalError
This is used to identify errors when using the global eval() function.
According to EcmaSpec 2018 edition:
This exception is not currently used within this specification. This object remains for compatibility with previous editions of this specification.

7. InternalError
This error occurs internally in the JS engine, especially when it has too much data to handle and the stack grows way over its critical limit.
This occurs when the JS engine is overwhelmed by too many recursions, too many switch cases, etc


