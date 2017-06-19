## _printf
_printf will produce output accrding to a format.
**Prototype:** _printf(const char *, ...);
## Tasks
Number | Description
------ |  ----------
0      |  Write function that produces output with conversion specifiers c, s, and %.
1      |  Handle conversion specifiers d, i.
2      |  Create a man page for your function.
3      |  Handle conversion specifier b.
4      |  Handle conversion specifiers u, o, x, X.
5      |  Use a local buffer of 1024 chars in order to call write as little as possible.
6      |  Handle conversion specifier S.
7      |  Handle conversion specifier p.
8      |  Handle flag characters +, space, and # for non-custom conversion specifiers.
9      |  Handle length modifiers l, h for non-custom conversion specifiers.
10     |  Handle the field width for non custom conversion specifiers.
11     |  Handle the precision for non-custom conversion specifiers.
12     |  Handle the 0 flag character for non-custom conversion specifiers.
13     |  Handle the - flag character for non-custom conversion specifiers.
14     |  Handle the custom conversion specifier r that prints the reversed string.
15     |  Handle the custom conversion specifier R that prints the rot13'ed string.
16     |  All above options should work well together.

## USES
**String:** ```
	    _printf("%s\n", "This is a string.");
	    ```
**Output:** This is a string.

**Character:** ```
	       _printf("%c\n", "V");
	       ```
**Output:** V

**Integer:** ```
	     _printf("%i\n", "10")
	     ```
**Output:** 10

**Decimal:** ```
	     _printf("%d\n", "1000")
	     ```
**Output:**  1000