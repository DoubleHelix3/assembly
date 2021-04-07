# Instruction Set

## Syntax

- Register acted on is the leftmost input

| Symbol | Meaning |
| :-: | -- |
| $ | Register |
| \# | Literal Value |
| \* | Register pointing to an address |

## General Purpose

General-purpose assembly instructions:

| Instruction | Description |
|--|--|
| HLT | Halts Execution |
| ZRG $ | Zero Register |
| PUT $ \#| Put a literal into a register |
| CP $ $ | Copy from one register to another|
| SWP $ $ | swap the values of two registers |

## Memory

| Instruction | Description |
|--|--|
| ZRM \* | Zero Memory pointed to by Register |
| ZRM \# | Zero Memory at literal address |
| LDA $ *| Load a memory value into a register |
| STA * $ | Load a memory value into a register |

## Arithmetic Operations

| Instruction | Description |
|--|--|
| ADD $ | Add to the accumulator |
| SUB $ | Subtract from the accumulator |
| MUL $ | Multiply the accumulator |
| DIV $ | Divide the accumulator |
| MOD $ | Put remainder into accumulator |
| INC | Increments the accumulator by 1 |
| DEC | DECREMENTS the accumulator by 1 |

## Bit Operations

| Instruction | Description |
|--|--|
| AND $| Bitwise AND the register with the accumulator |
| OR $| Bitwise OR the register with the accumulator |
| NOT | Bitwise NEGATE the accumulator |
| XOR $| Bitwise XOR the register with the accumulator |
| ROR $| Rotate Right by amount in register|
| ROL $| Rotate Left by amount in register|
| SHR $| Right shift by amount in register|
| SHL $| Left shift by amount in register|

## Comparison

| Instruction | Description |
|--|--|
| EQ $ $ | Equality of two register |
| NEQ $ $ | Inequality of two registers |
| LT $ $ | First register is less than the second instruction |
| LEQ $ $ | First register is less than the second instruction |
| GT $ $ | First register is greater than the second instruction |
| GEQ $ $ | First register is greater than the second instruction |

## Jumping

| Instruction | Description |
|--|--|
JMP \# | Unconditional Jump |
JMP \$ | Unconditional Jump |
JF \# | Jump forward |
JF \$ | Jump forward |
JB \# | Jump backwards |
JB \$ | Jump backwards |
JT \# | Conditional jump |
JT \$ | Conditional jump |
JTF \# | Conditional Jump forward |
JTF \$ | Conditional Jump forward |
JTB \# | Conditional Jump backwards |
JTB \$ | Conditional Jump backwards |
