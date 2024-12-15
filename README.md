# CST-405-Compiler
Written by Evan Lloyd and Spencer Meren

## Compilation and Execution

Bison and Flex must be installed in order to compile this program.

A Makefile is provided to easily compile and execute the parser.

- `make test1`, `make test2` ... `make test10` will compile and execute the program with a specific test program as a launch argument. Each test corresponds to a test program located in `/samples`. After execution, output logs, TACs, and the compiled MIPS code for the test program of choice will be located in `/outputs`
- `make clean` will delete all executables, object files, and output file

## Language Features

- Support for integer (`int`), single-point float (`float`), and character (`char`) variables
- Arithmetic operations
    - addition: `+`
    - subtraction: `-`
    - multiplication: `*`
    - division: `/`
    - modulus: `%`
- Comparison operators
    - greater than, less than (or equal to): `<`, `>`, `<=`, `>=`
    - equivalence: `=`
    - non-equivalence: `!=`
- Logical Operators
    - AND: `&&`
    - OR: `||`
    - NOT: `!`
- `if`-`elif`-`else` statements
- `while` statements
    - Includes `break` keyword to exit loop
- Functions
    - Return type
    - Arguments
    - Variable shadowing
    - Does not support local variables
- `write` statement

All statements which do not end in a block (defined as a series of statements surrounded by curly braces) should be separated by a semicolon (`;`)
