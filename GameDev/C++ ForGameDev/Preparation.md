# Preparation
- Hello world
- C/C++ file
- Entry point 
- C/C++ libraries
- Compile process

1. Hello world<br />
![helloworld](image.png)
2. C/C++ file
- Header file (.h)
    - aka include file
    - Hold declarations for other files use
(prototype)
    - Not required
- Source file (.c / .cpp)
    - Content implementation
    - Required <br />
![files](image-1.png)
3. Entry point 
- Required unique entry point
- The most common is: main<br />
![alt text](image-2.png)
4. C/C++ libraries
- C/C++ support a set of internal basic library, such as
    - Basic IO
    - Math
    - Memory handle
    - …
- For using, include the header file
    - #include <…>
    - #include "…"<br /> 
![alt text](image-3.png)
- [Reference](http://www.cplusplus.com/reference/)<br />
![alt text](image-4.png)
- C/C++ user-defined lib
    - Not C/C++ standard lib
    - Come from:
        - Third-party
        - User own
    - In common, include 2 parts
        - .h files & .lib files: for developer
        - .dll file (dynamic library): for end-user
    - For using
        - Include .h files
        - Inform .lib files to compiler
        - Copy all .dll file to (if any) :
            - same folder with execute file
            - to system32 (windows) – not recommend
- Declare path to .lib<br />
![alt text](image-5.png)
- Declare .lib file<br />
![alt text](image-6.png)
5. Compile process<br />
![alt text](image-7.png)
