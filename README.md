<p align="center">
  <img src="https://github.com/jotavare/jotavare/blob/main/42_banner/42_banner_ft_printf.png">
</p>

<p align="center">
	<img src="https://img.shields.io/badge/status-finished-success?color=%2312bab9&style=flat-square" />
	<img src="https://img.shields.io/badge/evaluated-18%20%2F%2012%20%2F%202022-success?color=%2312bab9&style=flat-square" />
	<img src="https://img.shields.io/badge/score-104%20%2F%20100-success?color=%2312bab9&style=flat-square" />
	<img src="https://img.shields.io/github/languages/top/jotavare/libft?color=%2312bab9&style=flat-square" />
	<img src="https://img.shields.io/github/last-commit/jotavare/libft?color=%2312bab9&style=flat-square" />
</p>

<p align="center">
	<a href="#about">About</a> •
	<a href="#how-to-use">How to use</a> •
	<a href="#mandatory">Mandatory</a> •
	<a href="#testers">Testers</a> •
	<a href="#license">License</a>
</p>

## ABOUT
As part of the 42 school curriculum, we are required to complete the ft_printf project, which involves recreating the well-known C library function, printf. This project provides a valuable learning opportunity in variadic arguments and structures, particularly if we intend to incorporate additional flags into our implementation of printf.

<a href="https://github.com/jotavare/ft_printf/blob/master/subject/en_subject_ft_printf.pdf">Click here</a> for the subject of this project.

## HOW TO USE
#### COMPILE
#### 1º - Clone the repository
```bash
git clone git@github.com:jotavare/ft_printf.git
```
#### 2º - Enter the project folder and run `make`
```bash
cd ft_printf\ft_printf
make
```

#### MAKEFILE RULES

``make`` or ``make all`` - Compile ft_printf.

``make clean`` - Delete all .o (object files) files.

``make fclean`` - Delete all .o (object files) and .a (executable) files.

``make re`` - use rules `fclean` + `all`

## MANDATORY
This ft_printf function supports several format specifiers, described below.

* ``%c`` - Prints a single character
* ``%s`` - Prints a string
* ``%p`` - Prints a pointer adress
* ``%d`` or ``%i`` - Prints a signed integer
* ``%u`` - Prints an unsigned integer
* ``%x`` or ``%X`` - Prints an unsigned integer in hexadecimal format

## DISCLAIMER
At 42School, almost every project must be written in accordance to the Norm, the schools' coding standard.

```bash
- No for, do while, switch, case or goto are allowed
- No more than 25 lines per function and 5 functions per file
- No assigns and declarations in the same line (unless static)
- No more than 5 variables in 1 function
... 
```

<a href="https://github.com/jotavare/libft/blob/master/subject/en_subject_ft_printf.pdf">Click here</a> for more information on 42 norm.

## TESTERS
* [Francinette](https://github.com/xicodomingues/francinette)
* [printfTester](https://github.com/Tripouille/printfTester)

## LICENSE
<p>
This work is published under the terms of <a href="https://github.com/jotavare/jotavare/blob/main/LICENSE">42 Unlicense</a>.
</p>
