
<h1><b> Printf </b></h1>


<b>Resources</b>

<a href="https://s3.eu-west-3.amazonaws.com/hbtn.intranet/uploads/misc/2022/11/d38f88e96a617135804dca9f9c49632751e06aa7.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA4MYA5JM5DUTZGMZG%2F20230313%2Feu-west-3%2Fs3%2Faws4_request&X-Amz-Date=20230313T003259Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=03f267a6bae2fd1dc0533a884cbfa9b67ff43370e2bec3bf8b18698793eacb90"> Secrets of printf</a>

<br><a href="https://www.it.uc3m.es/pbasanta/asng/course_notes/input_output_printf_en.html#:~:text=8.3.-,4.,be%20printed%20on%20the%20screen"> The printf function</a>

<b>Learning Objectives</b>
At the end of this project, you are expected to be able to explain to anyone, without the help of Google:

<b>Requirements</b>

General

<br>-Allowed editors: vi, vim, emacs
<br>-All your files will be compiled on Ubuntu 20.04 LTS using gcc, using the options -Wall -Werror -Wextra -pedantic -std=gnu89
<br>-All your files should end with a new line
<br>-A README.md file, at the root of the folder of the project is mandatory
<br>-Your code should use the Betty style. It will be checked using betty-style.pl and betty-doc.pl
<br>-You are not allowed to use global variables
<br>-No more than 5 functions per file
<br>-In the following examples, the main.c files are shown as examples. You can use them to test your functions, but you don’t have to push them to your repo (if you do we won’t take them into account). We will use our own main.c files at compilation. Our main.c files might be different from the one shown in the examples
<br>-The prototypes of all your functions should be included in your header file called main.h
<br>-Don’t forget to push your header file
<br>-All your header files should be include guarded
<br>-Note that we will not provide the _putchar function for this project

<b>Description</b>

The printf function (the name comes from “print formatted”) prints a string on the screen using a “format string” that includes the instructions to mix several strings and produce the final string to be printed on the screen.    A custom _printf() for learning purposes was developed by cohort #20 students Sarah Markland and Carlos Alarcon.  _printf() function format string is a character string, beginning and ending in its initial shift state, if any. These arguments are placed using the percentage '%' operator

 
<b>Your code will be compiled this way: </b>

<br>$ gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c

<br>As a consequence, be careful not to push any c file containing a main function in the root directory of your project (you could have a test folder containing all your tests files including main functions)
<br>Our main files will include your main header file (main.h): #include main.h
<br>You might want to look at the gcc flag -Wno-format when testing with your _printf and the standard printf. Example of test file that you could use:

<b>Use & Examples </b>

<br>Prototype: int _printf(const char *format, ...); Use - General: _printf("format string", var1, var2, ...);

<br>Examples:

<br>Basic String: _printf("%s Holberton", "Hello");`

<br>Output: Hello Holberton

<br>Print integers: _printf("This is an array element: arr[%d]:%c", 32, arr[32]);`

Output: This is an array element arr[32]:A


<b>Files contained in this repository</b>

<TABLE BORDER>
	<TR>
		<TH>Name</TH> <TH>Information</TH> <TH>Relevant Files</TH>
	</TR>
	<TR>
		<TD>man_3_printf</TD> <TD>Man page of the _printf() function.</TD> <TD>None</TD>
	</TR>
	<TR>
		<TD>main.h</TD> <TD>Header file with the data type struct, standard libraries and custom prototypes.</TD> <TD>*.c compilation</TD>
	</TR>
        <TR>
		<TD>_printf.c</TD> <TD>Main printf function file. Calls other functions.</TD> <TD>printf_(name of var).c file</TD>
	</TR>
        <TR>
		<TD>printf_37.c</TD> <TD>Contains percentage print function.</TD> <TD>None</TD>
	</TR>
        <TR>
		<TD>printf_int.c</TD> <TD>Contains decimal and integer functions.</TD> <TD>None</TD>
	</TR>
        <TR>
		<TD>printf_char.c</TD> <TD>Custom function for char data type.</TD> <TD>None</TD>
	</TR>
        <TR>
		<TD>printf_string.c</TD> <TD>Function that calls string type variable.</TD> <TD>None</TD>
	</TR>
         <TR>
		<TD>printf_str.c</TD> <TD>Auxiliar functions such as strlen and strcpy.</TD> <TD>None</TD>
	</TR>
        <TR>
		<TD>_putchar.c</TD> <TD>Custom putchar function.</TD> <TD>None</TD>
	</TR>   
</TABLE>

<b>Tasks required for this project</b>

0. I am not going anywhere. You can print that wherever you want to. I'm here and I am a Spur for life1. I am not going anywhere. You can print that wherever you want to. I'm here and I am a Spur for life.

<br>Write a function that produces output according to a format. Handle the following conversion specifiers:

<br>*c
<br>*s
<br>*%

<br>1. Education is when you read the fine print. Experience is what you get if you dont
Handle the following conversion specifiers:

*d
*i

<br>2. Just because its in print doesn't mean its the gospel
Create a man page for the function
