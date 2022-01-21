<h1 align="center">
	🧰 ft_printf
</h1>

<p align="center">
	<b><i>Because putnbr and putstr aren’t enough</i></b><br>
</p>

<p align="center">
	<img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/abdulazizabduvakhobov/ft_printf?color=lightblue" />
	<img alt="Number of lines of code" src="https://img.shields.io/tokei/lines/github/abdulazizabduvakhobov/ft_printf?color=critical" />
	<img alt="Code language count" src="https://img.shields.io/github/languages/count/abdulazizabduvakhobov/ft_printf?color=yellow" />
	<img alt="GitHub top language" src="https://img.shields.io/github/languages/top/abdulazizabduvakhobov/ft_printf?color=blue" />
	<img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/abdulazizabduvakhobov/ft_printf?color=green" />
</p>

<h3 align="center">
	<a href="#%EF%B8%8F-about">About</a>
	<span> · </span>
	<a href="#%EF%B8%8F-usage">Usage</a>
	<span> · </span>
  <a href="#usefull-make-command">Usefull Command</a>
	<span> · </span>
	<a href="#-testing">Testing</a>
</h3>

---

## 💡 About the project

> _This project is pretty straight forward. You will recode printf. Hopefully you will be able to reuse it in future project without the fear of being flagged as a cheater. You will mainly learn how to use variadic arguments._

### What is ft_printf?
ft_printf is an individual project at [42](https://www.42istanbul.com.tr/) that requires us to create a function similar to the printf from <stdio.h>. The function ft_printf() (the name comes from “print formatted”) prints a string on the screen using a “format string” that includes the instructions to mix several strings and produce the final string to be printed on the screen.

### Application flow
Click [here](https://excalidraw.com/#json=X5IF2CEVuO8EhAyX9bwMZ,42SQg0D6nJcF7hwcDG1dVw) for the interactive link.

#### Objectives
- Unix logic

#### Skills
- Rigor
- Unix
- Algorithms & AI

#### My grade
<img src="./images/grade.png" width="150" height="150"/>

## List of functions:

* [`ft_convert`](/sources/ft_convert.c)			- converts num to related numerical base.
* [`ft_putnbr`](/sources/ft_putnbr.c)			  - prints the number on the screen.
* [`ft_putstr`](/sources/ft_putstr.c)			  - prints given string on the screen.
* [`ft_putchar`](/sources/ft_putstr.c)			- prints given character on the screen.
* [`ft_putunbr`](/sources/ft_putunbr.c)			- prints given number on the screen (only positive).
* [`ft_putptr`](/sources/ft_putptr.c)			- prints given data by hexidecimal numerical base on the screen
* [`ft_strlen`](/sources/ft_strlen.c)			  - computes length of given string.
* [`ft_printf`](/sources/ft_printf.c)			  - prints a string on the screen using a “format string” that includes the instructions to mix several strings and produce the final string to be printed on the screen.


## 🛠️ Usage

**Follow the steps below**

### Instructions

**1. Clone the repository from github**

```bash
git clone https://github.com/abdulazizabduvakhobov/ft_printf && cd ft_printf/
```
**2. Compile the library by Makefile**
To compile the library, go to its path and run:

For all mandatory functions:

```bash
 make
```

**3. Create main.c to test the funtion:**
```bash
touch main.c
```

**4. Using it in your code**

To use the function in your code, simply include its header:

```C
#include "ft_printf.h"
```

**Example of a main**
```C
#include "ft_printf.h"

int main(void)
{
  ft_printf("%s", "Hello World");
  ft_printf("%c", '\n');
  ft_printf("%d", 123456789);
  ft_printf("%c", '\n');
  ft_printf("%X", 987654321);
 return (0);
}

/**
* output: 
* Hello World
* 123456789
* 3ADE68B1
**/
```

**5.After coding, you have to compile your code with libftprintf.a library like an example below**

```bash
gcc main.c libftprintf.a && ./a.out
# Done :)
```

### Requirements

The library is written in C language and needs the **`gcc` compiler** and some standard **C libraries** to run.

## Usefull make command

**1. Cleaning all binary (.o) files**

To clean all files generated binary files while doing a make, go to the path and run:

```bash
 make clean
```

**2. Cleaning all binary (.o) and executable files (.a)**

To clean all files generated while doing a make, go to the path and run:

```bash
 make fclean
```

**2. Checking Norminette standart**

To check Norminette errors of all files, simply go to the path and run:

```bash
 make norm
```

**3. Help command**

To get information about command, run:

```bash
 make help
```

## 📋 Testing

You can use any of this third party testers to test the project

* [Tripouille/printfTester](https://github.com/Tripouille/printfTester)
* [paulo-santana/ft_printf_tester](https://github.com/paulo-santana/ft_printf_tester)
