# Monty

Monty 0.98 is a scripting language that is first compiled into Monty byte codes (Just like Python). It relies on a unique stack, with specific instructions to manipulate it. The goal of this project is to create an interpreter for Monty ByteCodes files.

This project was built by Hugo Bayona and Alejo López

# Table of Contents

1. [Authors](#Authors)
2. [Features](#Features)
3. [How Use](#How-Use)
4. [Brainfuck](#Brainfuck)

# Authors

👤 **Kafui Kumah**

- Twitter: [@alejolo311](https://twitter.com/kafuikumah_)
- Github: [@alejolo311](https://github.com/kafuikumah)

# Features

The following opcodes are suported.

- (push) Push an integer to the stack.
- (pall) Prints the entire stack.
- (pint) Print the first element of the stack.
- (pop) Removes the top element of the stack.
- (swap) Swaps the top two elements of the stack.
- (add, sub, mul, div, mod) Aritmetic op +, -, \*, /, %.
- (nop)
- (pchar) Prints the char at the top of the stack, followed by a new line.
- (pstr) Prints the string starting at the top of the stack, followed by a new line.
- (rotl) Rotates the stack to the top.
- (rotr) Rotates the stack to the bottom.
- (stack) Sets the format of the data to a stack (LIFO). DEFAULT.
- (queue) Sets the format of the data to a queue (FIFO).

# How Use

## How to compile

$ gcc -Wall -Werror -Wextra -pedantic \*.c -o monty

### Requirements

- compile on Ubuntu 14.04 LTS
- compile with gcc 4.8.4

### Examples

```bash
$ cat -e bytecodes/00.m
push 1$
push 2$
push 3$
pall$
$ ./monty bytecodes/00.m
3
2
1
$
```

# Brainfuck

Brainfuck is an esoteric programming language created in 1993 by Urban Müller, and is notable for its extreme minimalism.

This repository includes 4 files with Brainfuck implementations.

- A Brainf\*ck script that prints School, followed by a new line.
- Add two digits given by the user.
- Multiply two digits given by the user.
- Multiply two digits given by the user + print a new line at the end.

## How to compile

$ bf ./1001-add.bf

### Requirements

- compile on Ubuntu 14.04 LTS
- compile with bf

```bash
$ apt-get install bf
```

