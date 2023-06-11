<p align="center">
  <img src="https://github.com/jotavare/jotavare/blob/main/42/banner/new/42_ft_printf_banner_new.png">
</p>

<p align="center">
	<img src="https://img.shields.io/badge/status-finished-success?color=%2312bab9&style=flat-square" />
	<img src="https://img.shields.io/badge/evaluated-22%20%2F%2012%20%2F%202022-success?color=%2312bab9&style=flat-square" />
	<img src="https://img.shields.io/badge/score-104%20%2F%20100-success?color=%2312bab9&style=flat-square" />
	<img src="https://img.shields.io/github/languages/top/jotavare/ft_printf?color=%2312bab9&style=flat-square" />
	<img src="https://img.shields.io/github/last-commit/jotavare/ft_printf?color=%2312bab9&style=flat-square" />
	<a href='https://www.linkedin.com/in/joaoptoliveira' target="_blank"><img alt='Linkedin' src='https://img.shields.io/badge/LinkedIn-100000?style=flat-square&logo=Linkedin&logoColor=white&labelColor=0A66C2&color=0A66C2'/></a>
	<a href='https://profile.intra.42.fr/users/jotavare' target="_blank"><img alt='42' src='https://img.shields.io/badge/Porto-100000?style=flat-square&logo=42&logoColor=white&labelColor=000000&color=000000'/></a>
</p>

<p align="center">
	<a href="#about">About</a> •
	<a href="#how-to-use">How to use</a> •
	<a href="#mandatory">Mandatory</a> •
	<a href="#norminette">Norminette</a> •
	<a href="#license">License</a>
</p>

## ABOUT
As part of the 42 school curriculum, we are required to complete the ft_printf project, which involves recreating the well-known C library function, printf. This project provides a valuable learning opportunity in variadic arguments and structures, particularly if we intend to incorporate additional flags into our implementation of printf.

<a href="https://github.com/jotavare/ft_printf/blob/master/subject/en_subject_ft_printf.pdf">Click here</a> for the subject of this project.

## HOW TO USE
#### COMPILE
#### 1º - Clone the repository
```
git clone git@github.com:jotavare/ft_printf.git
```

#### 2º - Enter the project folder and run `make`
```
cd ft_printf\ft_printf
make
```

#### 3º - To use in your code, include the header
```
#include "ft_printf.h"
```

#### MAKEFILE RULES

`make` or `make all` - Compile ft_printf.

`make clean` - Delete all .o (object files) files.

`make fclean` - Delete all .o (object files) and .a (executable) files.

`make re` - use rules `fclean` + `all`.

## MANDATORY
This ft_printf function supports several format specifiers, described below.

* `%c` - Prints a single character
* `%s` - Prints a string
* `%p` - Prints a pointer adress
* `%d` or `%i` - Prints a signed integer
* `%u` - Prints an unsigned integer
* `%x` or `%X` - Prints an unsigned integer in hexadecimal format

## NORMINETTE
At 42 School, it is expected that almost every project is written in accordance with the Norm, which is the coding standard of the school.

```
- No for, do...while, switch, case, goto, ternary operators and variable lenght arrays are allowed
- Each function must be maximum 25 lines, not counting the function's own curly brackets
- Each line must be at most 80 columns wide, comments included
- A function can take 4 named parameters maximum
- No assigns and declarations in the same line (unless static)
- You can't declare more than 5 variables per function
- ...
```

<a href="https://github.com/jotavare/jotavare/blob/main/42/pdf/en_norm.pdf">Click here</a> for more information on 42 norms.

## LICENSE
<p>
This work is published under the terms of <a href="https://github.com/jotavare/jotavare/blob/main/LICENSE">42 Unlicense</a>.
</p>
