# Compiler Lab Programs

Compiler Lab inte Kurchu Programs 😃
Code isttappettaal Star and Follow 😁😅    


## Project Structure

````markdown
# Made by Jibin Wilson S7 CSE

>

# Compiler Lab Programs

Compiler Lab inte Kurchu Programs 😃
Code isttappettaal Star and Follow 😁😅    



## Project Structure

```
├── README.md
├── AUTHORS.md        # Attribution and provenance
├── calculator/
│   ├── calc.l          # Lex file for calculator lexer
│   └── calc.y          # Yacc file for calculator parse
├── ConstantPropagation/
│   ├── const.c         # Constant propagation implementation
│   ├── input.txt       # Sample input for constant propagation
│   └── TestCase.txt    # Test cases for constant propagation
├── IntermediateCode/
│   └── incode.c        # Intermediate code generation implementation
├── lexicalAnalyzer/
│   ├── lexicalAnalyzerC/
│   │   ├── Analyzer.c  # Manual lexical analyzer in C
│   │   └── input.txt   # Sample input for lexical analyzer
│   └── lexicalAnalyzerLex/
│       ├── Analyzer.l  # Lexical analyzer using Flex
│       └── input.txt   # Sample input for lexical analyzer
├── RecursiveDecentParser/
│   └── parser.c        # Recursive descent parser implementation
├── SampleLexPrograms/
│   ├── evenOrOdd/
│   │   └── evenOrOdd.l # Lex program to check even/odd numbers
│   ├── FlamesGame/
│   │   └── FlamesGame.l # Lex program for FLAMES game
│   ├── InGeneral/
│   │   └── InGeneral.l # Template Lex program for custom functions
│   ├── NumberOfCharacters/
│   │   └── character.l # Lex program to count number of characters
│   ├── Palindrome/
│   │   └── palindrome.l # Lex program to check palindromes
│   └── PrimeNumber/
│       └── prime.l     # Lex program to check prime numbers
├── ShiftReduceParser/
│   ├── info.txt        # Information about shift-reduce parser
│   ├── input.txt       # Sample input for shift-reduce parser
│   ├── parserSimpleLogic.c # Simple logic shift-reduce parser
│   └── parserUsingExternalFile.c # Shift-reduce parser using external file
└── yaccPrograms/
    ├── ValidExp/
    │   ├── ValidExp.l  # Lex file for valid expression
    │   └── ValidExp.y  # Yacc file for valid expression
    └── ValidIdentifier/
        ├── Valid.l     # Lex file for valid identifier
        └── Valid.y     # Yacc file for valid identifier
```

## Notes

- Oru karyam ondu maximum ee programs run cheythu nokkane Errors okke eppozha vandiyum vilichu varunnathu ennu parayan pattathilla
- Ee programs run cheyyumbol enthenkilum Sambhavichal athinte utharavathi ithu cheytha njan alla ennu ariyichu kollunnu😁

## How to run
### Program having both LEX and YACC programs
```
bison -d fileName.y  
flex fileName.l        
gcc lex.yy.c y.tab.c -o calcn ## YACC inte program run cheyyumbol y.tab.c generate aakunundengil ee command use cheyyaam allengil (fileName.tab.c) ennu use cheyyane
# Compiler Lab Programs

![Compiler Lab Banner](https://img.shields.io/badge/Compiler-Lab-blue)

Made by: **Jibin Wilson — S7 CSE**  
Imported from: https://github.com/Jithu-9847/Compiler_Lab.git

Small, friendly collection of compiler-lab programs (Lex/Yacc/handwritten C) used for teaching and experimenting with lexical analysis, parsing and intermediate code generation.

---

## Quick links

- Authors: `AUTHORS.md`  
- Project structure: see below  
- How to run: short instructions with examples

## Table of Contents

1. About
2. Project structure
3. How to run (examples)
4. Notes
5. Contributing

---

## 1) About

This repo collects small lab programs for compiler construction topics: lexical analyzers (Flex/lex), parsers (Bison/Yacc or recursive descent), shift-reduce parsing demo, and small supporting tools (constant propagation, intermediate code snippets).

The code is intentionally simple and educational — ideal for experimentation during lab sessions.

## 2) Project structure

Top-level layout (high level):

```
├── AUTHORS.md
├── README.md
├── calculator/                # small calc lexer+parser examples
├── ConstantPropagation/      # constant propagation examples in C
├── IntermediateCode/         # intermediate code generation examples
├── lexicalAnalyzer/          # lex examples (manual and flex)
├── RecursiveDecentParser/    # recursive descent parser
├── SampleLexPrograms/        # many small lex sample programs
├── ShiftReduceParser/        # shift-reduce parser demos
└── yaccPrograms/             # yacc/bison example programs
```

Explore folders to find small runnable examples and input files. Each program directory usually contains an input file and brief comments describing usage.

## 3) How to run — quick examples

Prerequisites: `gcc`, `flex` (or `lex`), `bison` (or `yacc`) installed on your system.

- Example: build a program using both Bison and Flex

```powershell
bison -d fileName.y
flex fileName.l
gcc lex.yy.c y.tab.c -o program
./program
```

- Example: build a Flex-only program

```powershell
flex fileName.l
gcc lex.yy.c -o lexer
./lexer
```

- Example: compile a plain C program

```powershell
gcc fileName.c -o program
./program
```

Tip: many sample programs include an `input.txt` file — run the produced executable and provide input via stdin or redirect from the sample input file.

## 4) Notes

- The programs are educational; they may not be production hardened. Expect small errors when porting across compilers — test and adapt as needed.  
- If you find a bug, feel free to open an issue or submit a pull request.

Small friendly message in original language:  
"Oru karyam ondu maximum ee programs run cheythu nokkane Errors okke eppozha vandiyum vilichu varunnathu ennu parayan pattathilla — Ee programs run cheyyumbol enthenkilum Sambhavichal athinte utharavathi ithu cheytha njan alla ennu ariyichu kollunnu 😁"

## 5) Contributing

Contributions welcome — add more examples, improve documentation or fix bugs. See `AUTHORS.md` for attribution.

---

If you'd like, I can also:

- add a small per-file header to each source file with the "Made by Jibin Wilson S7 CSE" attribution, or
- add a demo workflow (PowerShell script) to build and run the common examples.
