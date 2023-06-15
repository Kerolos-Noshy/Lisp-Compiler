# Lisp-Compiler
## Overview
This is a group project for a Lisp scanner and parser developed as part of Design of Compilers course. It aims to scan and analyze the structure of Lisp code and generate a parse tree representation. The parser is implemented in Python and uses the enum, re, pandas, tkinter, pandastable, and nltk libraries.

The parser consists of two main components: tokenization and parsing. The tokenization process involves identifying and categorizing different elements in the Lisp code, such as keywords, operators, identifiers, constants, and errors. The tokens are stored in a list for further processing.

The parsing process utilizes the tokens generated from tokenization to build a parse tree. The parse tree represents the hierarchical structure of the Lisp code, with each node in the tree corresponding to a specific component of the code. The parser uses recursive functions to traverse the tokens and construct the parse tree.

The code includes a graphical user interface (GUI) using the tkinter library in Python. The GUI allows users to input source code path and perform scanning and parsing operations on the code. Here's a description of the token stream window and the parse tree generated using the nltk library

## Usage
To use the parser, you need to run this code and enter the path of Lisp code as input. The code will be passed to the find_token function, which will tokenize the code and generate a list of tokens. These tokens can then be used as input to the parsing functions to build the parse tree.

You can modify the parser code to add additional parsing rules or handle specific Lisp constructs as needed. The provided code serves as a starting point for developing a more comprehensive Lisp parser.

## Futures
- Error Handling: Improve the error reporting and handling mechanism to provide more informative error messages when encountering invalid Lisp code.
- Token Stream: The token stream window displays the lexemes (individual tokens) extracted from the source code and their corresponding types. It provides a tabular view of the token stream, showing each lexeme and its associated token type. The token types can include keywords, operators, identifiers, constants, and errors.
- Parse Tree: The parse tree represents the hierarchical structure of the parsed Lisp code. the parse tree is generated using the nltk library. It represents the relationships between different components of the Lisp code, such as program structures, lists, and atoms.

## Sample use
here is a lisp code we will test it and see the results
```
; write Lisp Program to calculate factorial
(setq  c  1)
(setq  fact  1)
(dotimes (n  4)
  ( setq fact (* fact c) )(incf c) (write c) )
(Write fact)
 (write ”finished”)
; the code is finished
```
### Screen Shots
![image](https://github.com/Kerolos-Noshy/Lisp-Compiler/assets/101178275/ce3d3f1c-eb0d-4fd9-930b-2adf43189cbe)
- *write the path of the previous lisp code*

![image](https://github.com/Kerolos-Noshy/Lisp-Compiler/assets/101178275/06235530-4a25-413f-8361-0ad0da5c8a2b)
- *Error List*

![image](https://github.com/Kerolos-Noshy/Lisp-Compiler/assets/101178275/e4624248-2d07-4824-bcb3-88aecc5ee451)
- *Token Stream*

![image](https://github.com/Kerolos-Noshy/Lisp-Compiler/assets/101178275/98517515-6bc0-4eb2-9b82-86077f1e1464)
- *Parse Tree*




