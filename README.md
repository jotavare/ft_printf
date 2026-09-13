<p align="center">
  <img src="https://github.com/jotavare/jotavare/blob/main/42/banners/piscine_and_common_core/github_piscine_and_common_core_banner_ft_printf.png">
</p>

<p align="center">
	<img src="https://img.shields.io/badge/status-finished-success?color=%2312bab9&style=flat-square"/>
	<img src="https://img.shields.io/badge/evaluated-22%20%2F%2012%20%2F%202022-success?color=%2312bab9&style=flat-square"/>
	<img src="https://img.shields.io/badge/score-104%20%2F%20100-success?color=%2312bab9&style=flat-square"/>
	<img src="https://img.shields.io/github/languages/top/jotavare/ft_printf?color=%2312bab9&style=flat-square"/>
	<img src="https://img.shields.io/github/last-commit/jotavare/ft_printf?color=%2312bab9&style=flat-square"/>
	<a href='https://www.linkedin.com/in/jotavare' target="_blank"><img alt='Linkedin' src='https://img.shields.io/badge/LinkedIn-blue?style=flat-square'/></a>
	<a href='https://profile.intra.42.fr/users/jotavare' target="_blank"><img alt='42' src='https://img.shields.io/badge/Porto-100000?style=flat-square&logo=42&logoColor=white&labelColor=000000&color=000000'/></a>
</p>

<p align="center">
	<a href="#about">About</a> •
	<a href="#how-to-use">How to use</a> •
	<a href="#mandatory">Mandatory</a> •
	<a href="#bonus">Bonus</a> •
	<a href="#norminette">Norminette</a> •
	<a href="#debugging">Debugging</a> •
	<a href="#contributing">Contributing</a> •
	<a href="#license">License</a>
</p>

## ABOUT
This project involved recreating the well-known C library function, printf. This provided a valuable learning opportunity in variadic arguments and structures, particularly if we intend to incorporate additional flags into our implementation of print.

> [!NOTE]
> For the rest of the projects and exams in the cursus, <a href="https://github.com/jotavare/42-common-core">click here</a>.

## HOW TO USE
#### 1º - Clone the repository
```git
git clone git@github.com:jotavare/ft_printf.git
```

#### 2º - Enter the project folder and run `make`
```bash
cd ft_printf/ft_printf
make
```

#### 3º - To use in your code, include the header
```c
#include "ft_printf.h"
```

#### MAKEFILE RULES

`make` or `make all` - Compile ft_printf files.

`make clean` - Delete all .o (object files) files.

`make fclean` - Delete all .o (object files) and .a (executable) files.

`make re` - Use rules `fclean` + `all`.

## MANDATORY
> This ft_printf function supports several format specifiers, described below:
- [x] `%c` - Print a single character;
- [x] `%s` - Print a string;
- [x] `%p` - Print void * pointer argument in hexadecimal format;
- [x] `%d` - Print a decimal (base 10) number;
- [x] `%i` - Print an integer in base 10;
- [x] `%u` - Prints an unsigned decimal (base 10) number;
- [x] `%x` - Print a number in hexadecimal (base 16) lowercase format;
- [x] `%X` - Print a number in hexadecimal (base 16) uppercase format;
- [x] `%%` - Print a percentage sign;

## BONUS
- [ ] Manage any combination of the following flags: `-O` and the field minimum width under all conversions;
- [ ] Manage all the following flags: `#` ` ` `+`;

## NORMINETTE
> At 42 School, it is expected that almost every project is written following the Norm, which is the coding standard of the school.

```
- No for, do...while, switch, case, goto, ternary operators, or variable-length arrays allowed;
- Each function must be a maximum of 25 lines, not counting the function's curly brackets;
- Each line must be at most 80 columns wide, with comments included;
- A function can take 4 named parameters maximum;
- No assigns and declarations in the same line (unless static);
- You can't declare more than 5 variables per function;
- ...
```

* [42 Norms](https://github.com/42School/norminette/blob/master/pdf/en.norm.pdf) - Information about 42 code norms. `PDF`
* [Norminette](https://github.com/42School/norminette) - Tool to respect the code norm, made by 42. `GitHub`
* [42 Header](https://github.com/42Paris/42header) - 42 header for Vim. `GitHub`

## DEBUGGING
> Conversions are written straight to the file descriptor rather than into a
> buffer, so the things that go wrong here are a miscounted return value and a
> pointer read that runs past its argument.

Compile with `-g` to keep the symbols the debuggers need:

```bash
cc -Wall -Wextra -Werror -g main.c libftprintf.a
```

`valgrind --leak-check=full ./a.out` - Report memory that was allocated and never freed; the number and pointer conversions allocate while building their output.

`valgrind --track-origins=yes ./a.out` - Trace an uninitialised value back to where it came from, which is what a wrong `va_arg` type looks like.

`gdb ./a.out` - Step through a conversion and watch the running character count.

`cc -fsanitize=address -g ...` - Catches leaks and out-of-bounds reads without valgrind, and runs much faster.

The return value has to match what the real `printf` reports, so compare both on
the same format string rather than only looking at what is printed. `INT_MIN`,
an empty string and `%%` are the usual places an implementation disagrees.

* [GDB](https://www.sourceware.org/gdb/) - The GNU debugger. `Website`
* [Valgrind](https://valgrind.org/docs/manual/quick-start.html) - Quick start guide. `Website`

## CONTRIBUTING

This repository documents work already submitted and graded, so it is not open
to changes. Feel free to fork it if any of it is useful to you.

## LICENSE

This project is available under the MIT License. For further details, please refer to the [LICENSE](https://github.com/jotavare/ft_printf/blob/main/LICENSE) file.
