Develop a lexical analyzer to recognize few patterns (like identifier,constants,comments,operators etc.)

Description This LEX program acts as a basic lexical analyzer, which scans the input and classifies tokens commonly found in C programs. It identifies keywords, identifiers, constants, operators, and comments.

What It Identifies

Keywords – Predefined reserved words like int, float, if, while, etc.
2.. Identifiers – Names defined by the user, starting with a letter followed by letters or digits.

Constants :– Integer constants: Numbers without a decimal point. Float constants: Numbers with a decimal point.

Operators: – Arithmetic: +, -, *, / Relational: <, >, <=, >=, !=, == Logical: &&, ||, ! Bitwise: &, <<, >>, ^ Assignment: =

Comments – Single-line comments starting with //.

How It Works:

The definition section uses regular expressions to define patterns for different token types. The rules section matches the input against these patterns and prints the type of token found: Example: If the input matches {keyword}, it prints is a keyword. The user code section contains main() which calls yylex() to start tokenizing.
