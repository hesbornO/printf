## _printf
_printf will produce output according to a format.
**Prototype:** _printf(const char *, ...);
## Requirements
* All files will be compled on Ubuntu 14.04 LTS
* Programs and functions will be compiled with gcc 4.8.4 using flags -Wall -Werror -Wextra and -pedantic
* All files should end in a new line
* Code should use the [Betty](https://github.com/holbertonschool/Betty/wiki) style
* Global variables are not allowed
* No more than 5 functions per file
* main.c are shown as examples and files can be used to test your functions
* The prototypes of all functions should be included in the header file called holberton.h
* All header files should be include guarded
* Authorized functions and macros:
  * write (man 2 write)
  * malloc (man 3 malloc)
  * free (man 3 free)
  * va_start (man 3 va_start)
  * va_end (man 3 va_end)
  * va_copy (man 3 va_copy)
  * va_arg (man 3 va_arg)
## Mandatory Tasks
Number | Description | Completion Status
------ |  ---------- | ---------
0     |  Write function that produces output with conversion specifiers c, s, and %. | Completed
1     |  Handle conversion specifiers d, i. | Completed
2     |  Create a man page for your function. | Completed
## Advanced Tasks
Number | Description | Completion Status
------ |  ---------- | ---------
3     |  Handle conversion specifier b. | Completed
4     |  Handle conversion specifiers u, o, x, X. | Completed 
5     |  Use a local buffer of 1024 chars in order to call write as little as possible. | Incomplete
6     |  Handle conversion specifier S. | Completed 
7     |  Handle conversion specifier p. | Completed 
8     |  Handle flag characters +, space, and # for non-custom conversion specifiers. | Incomplete
9     |  Handle length modifiers l, h for non-custom conversion specifiers. | Incomplete
10    |  Handle the field width for non custom conversion specifiers. | Incomplete
11    |  Handle the precision for non-custom conversion specifiers. | Incomplete
12    |  Handle the 0 flag character for non-custom conversion specifiers. | Incomplete
13    |  Handle the - flag character for non-custom conversion specifiers. | Incomplete
14    |  Handle the custom conversion specifier r that prints the reversed string. | Completed
15    |  Handle the custom conversion specifier R that prints the rot13'ed string. | Completed
16    |  All above options should work well together. | Incomplete
## File Descriptions
* **_printf.c:** This file uses the prototype ```int _printf(const char *format, ...);``` and format is a character string. The format string is composed of zero or more directives. See ```man 3 printf``` for more detail. _printf will return the number of characters printed (excluding the null byte used to end output to strings) and will write output to stdout, the standard output stream.
* **_putchar.c:** This file uses the prototype ```int _putchar(char c);```that  writes a char specified by the argument to stdout.
* **holberton.h:** This file contains all function prototypes used throughout this assignment.
* **man_3_printf:** This is the man page for our custom _printf function.
* **print_chars.c:** This file uses function prototype ```int print_c(va_list c);``` to handle the conversion specifier ```c``` which converts the int argument to a char, and the resulting character is written. Function prototype ```int print_s(va_list s);``` is also used in this file to handle the conversion specifier ```s``` which expects the ```char *``` argument to be a pointer to an array of character type (pointer to a string) and prints the string.
* **print_numbers.c:** This file contains the function prototypes ```int print_i(va_list i);``` and ```int print_d(va_list d);``` these functions handle the conversion specifiers ```d``` and ```i``` which convert an int argument to a signed decimal notation.
* **print_hex.c:** Function prototype ```int print_hex(unsigned int n, unsigned int c);``` prints an unsigned int in hexidecimal form and will return the number of digits printed. This function is used as a helper to functions ```int print_x(va_list x)``` and ```int print_X(va_list X)``` which handle conversion specifiers ```x``` and ```X``` which take an unsigned int and print it in lowercase or uppercase hex notation. One more function prototype ```int print_p(va_list p);``` is included in this file and it handles conversion specifier ```p``` that prints an address.
* **print_unsigned_int.c:** this file uses function prototypes ```int print_u(va_list u);``` to handle conversion specifier ```u``` to print an unsigned int in decimal notation, ```int print_0(va_list o)``` to handle conversion specifier ```o``` to take an unsigned int and print it in octal notation, and ```int print_b(va_list b)``` to handle conversion specifier ```b``` that takes an unsigned int and prints it in binary notation.
## Uses
**String:** ```
	    _printf("%s\n", 'This is a string.');
	    ```
**Output:** This is a string.

**Character:** ```
	       _printf("%c\n", 'V');
	       ```
**Output:** V

**Integer:** ```
	     _printf("%i\n", 10);
	     ```
**Output:** 10

**Decimal:** ```
	     _printf("%d\n", 1000);
	     ```
**Output:**  1000
## Authors
Alexa Orrico [GitHub](https://github.com/alexaorrico) [Twitter](https://twitter.com/alexa_orrico)

Daniel Ojeda [GitHub](https://github.com/Danielo814) [Twitter](https://twitter.com/DanielC_Ojeda)
