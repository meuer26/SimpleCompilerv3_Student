## Simple Compiler v3

Dan O’Malley

A teaching compiler that uses a C-like input language, outputs LLVM IR, and then outputs x86-64 and ARM machine language. This is version 3. Version 1 available [here](https://github.com/meuer26/SimpleCompilerv1). This was written between 2023-2025 for teaching compiler concepts.

This teaching compiler's focus is low-level implementation details of lexing, parsing, codegen for a hand-rolled LLVM IR, and a multi-target hand-rolled backend (supporting x86-64 and AArch64). Modular front-end and back-end support an optimizer middle-end, optimizing the hand-rolled LLVM IR. No LLVM library dependencies. Outputs x86 and ARM assembly for nasm and aarch64-linux-gnu-as assemblers.


## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.


## Features

- Front-end supports C-like input language. This language includes: declarations, declarations with assignment, reassignment, assignment of unary and binary expressions, addition, subtraction, multiplication and logical negation, Less Than operator, do-while loops, increment, and return values. 
- Only 32-bit integers supported.
- Functions can take zero or one argument. Only one function per file is supported. A maximum of one do-while loop per function.
- Symbol table can support up to 100 entries.
- 300+ test cases for automated, parallel testing (including x86 and ARM test cases).




## Attribution

- Code and test cases written by Dan O'Malley between 2023-2025.
- Progress bar in run_all_test_cases_for_errors.sh was modified from [Baeldung](https://www.baeldung.com/linux/command-line-progress-bar) and that is noted in that file.
- Parallel testing code in run_all_test_cases_for_errors.sh was written by Grok v4 (xAI) and that is noted in that file. 