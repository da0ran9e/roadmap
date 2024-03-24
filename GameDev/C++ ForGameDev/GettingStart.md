# Getting start
- Variables and constant
- Primary data type
- Array –String
- Data structure: enum–struct
- Function
- Namespace

## Variables and constant <br />
![alt text](image-8.png)
1. Auto variable:
- As default, a variable is a auto variable
```C++
int myVar
/* is actually */
auto int myVar
```
- Go out of scope once the program exits from the current block
2. Static variable:
- Allocated when the program starts and is
deallocated when the program ends.
- Default value is zero(0)<br />
![alt text](image-9.png)
![alt text](image-10.png)
3. Register variable:
- Stored in a machine register if possible
- Usually used in “for iterator” for improve
performance <br />
![alt text](image-11.png)
4. Extern variable:
- Specify that the variable is declared in a
different file.
- Compiler will not allocate memory for the
variable
- Avoid duplicate declaration
- Share (global) variable for multiple .cpp files <br />
![alt text](image-12.png)
![alt text](image-13.png)
5. Constant:
- Variable's value is constant
- To prevent the programmer from modifying<br />
![alt text](image-14.png)

## Primary data type<br />
![alt text](image-15.png)
1. New type definition <br />
![alt text](image-16.png)
2. `sizeof` operator
- Return size (in byte) of a type, data structure, variable
```C++
int sizeInt = sizeof(int);
int sizeLong = sizeof(long);
```

## Array –String
1. Array
- Used to store consecutive values of the same data types <br />
`int b[4] = {1, 2, 3, 4};`
- N-dimensions array <br />
`int b[<s1>][<s2>]…[<sn>]` `si` MUST BE constant
- Index of array is counted from 0 to(si-1)
- C/C++ do not handle out-of-range exception <br />
![alt text](image-17.png)
2. Array Assignment <br />
![alt text](image-18.png)
3. Array Assignment 2D Array <br />
![alt text](image-19.png)
4. C/C++ String
- No standard string in C/C++
- Use char*, or char[] instead
- String in C/C++ is array of byte, end with ‘\0’<br />
![alt text](image-20.png)
5. String allocation
- Static allocation
```C++
char *st = "String";
char st2[] = "String";
```
- Dynamic allocation
```C++
char *st3 = new char[6];
st3[0] = 's';
st3[1] = 't';
st3[2] = 'i';
st3[3] = 'n';
st3[4] = 'g';
st3[5] = '\0';
```
![alt text](image-21.png)
## Data structure: enum–struct
1. Enum
- Use for set up collections of named integer constants
    - In traditional C way: <br />
    ![alt text](image-22.png)
    - Alternate approach <br />
    ![alt text](image-23.png)
- Declaration <br />
![alt text](image-24.png)
- Values of enum constants <br />
![alt text](image-25.png)
2. Struct
- Define a structure type and/or a variable of a structure type<br />
- ![alt text](image-26.png)
- Using struct: <br />
![alt text](image-27.png)
3. Struct-function <br />
![alt text](image-28.png)
- **C++ only, not available in C**
- Beside variable, struct also has had function
- Struct alignment is not effected to struct-function
- Function is not counted when calculate struct
size<br />
![alt text](image-29.png)
4. Struct constructor / destructor
- C++ only, not available in C
- Two special function of struct
    - Constructor: automatically call when a instant of structis created
    - Destructor: automatically call when a instant of structis destroy <br />
![alt text](image-30.png)
![alt text](image-31.png)
5. Structand static member
- Static function & static variable
- Static variable is not counted is struct alignment and struct size <br />
![alt text](image-32.png)
6. Structand Access privilege
- C++ only, not available in C
- Three access privilege methods
    - public: visible for all
    - private: visible inside struct only
    - protected: visible inside structand
retrieved struct(OOP)
- Default is public
- For example: valxis public <br />
![alt text](image-33.png)
## Function<br />
<return-type> function_name([<type> <param>], […]) <br />
![alt text](image-34.png)
1. Default parameters <br />
![alt text](image-35.png)
![alt text](image-36.png)
2. Variable number of parameters <br />
![alt text](image-37.png)
3. Parameter classification <br />
- Value parameter
- Reference parameter
- Constant parameter
- Const Reference parameter
- Pointer parameter
***Value parameter***
- Pass-by-value
- A copy of parameter is made <br />
![alt text](image-38.png)
* **Reference parameter**
- Pass-by-reference
- Actually parameter itself is passed
- Use reference operator “&” <br />
![alt text](image-39.png)
*** Constant parameter**
- Pass-by-value
- A copy of parameter is made and strict as const. <br />
![alt text](image-40.png)
*** Const Reference parameter**
- Pass-by-ref
- Actually parameter itself is passed but avoid modify
- Avoid the overhead of creating a copy<br />
![alt text](image-41.png)
*** Pointer parameter**
- In common, Pass-by-value
- A copy of parameter is made <br />
Value of parameter is an address of a memory block <br />
![alt text](image-42.png)
- Value of parameter will not be change,
- but memory block which pointed by parameter could be modified
4. Function overloading
- C++ only
- Allow multiple functions with the same name, so long as they have different parameters <br />
![alt text](image-43.png)
5. Function Prototype
- In C/C++, functions MUST BE declare before using.
- To solve this problems
    - Keep all functions in correct order
    - Use prototype inside .cpp file
    - Use prototype inside header (.h) file -> recommend <br />
    ![alt text](image-44.png)
6. Extern function
- Sometimes, we need to use a function in another module (.cppfile)
- Header file is too complicated to use (caused error when used) <br />
![alt text](image-45.png)
7. Inline function
- Macro: preprocessor replaces all macro calls directly with the macro code <br />
![alt text](image-46.png)
- Like macro, but obeys C/C++ syntax
![alt text](image-47.png)
- For OOP ,Inline function is allowed to set access privilege
- Improve performance (for short/simple inline functions)
- NOTE: The compiler is not forced to inline anything at all
## Namespace
1. Namespace:
- A abstract container uses for grouping source code.
- In C++, a namespace is defined with a namespace block <br />
![alt text](image-48.png)
2. Using namespace
- For using methods, variables, … of a namespace:
`<namespace>::<methods/variables>` <br />
![Using namespace](image-49.png)
![Use using namespace for shorten way](image-50.png)
3. Namespace –ambiguous call <br />
![alt text](image-52.png)
- More than two definition of add functions
    - maths::add()
    - matrix::add()
> ambiguous call fatal error. 
![alt text](image-51.png)
- In this case, MUST BE specify namespace. <br />
![alt text](image-53.png)
# Reference 
[cppreference.com](https://en.cppreference.com/w/)
[cplusplus.com](http://www.cplusplus.com/reference/)