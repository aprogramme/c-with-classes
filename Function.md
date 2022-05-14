

# Function in C++

1. Function is block of code performing a unit task.

2. Function has a name, return type and arguments.

3. Function is a way too achieve modularization.

4. Function are predefined and user-defined.

5. Predefined function are declared in header files and defined in libraruy file.

## Definition, Declaration and Call

```cpp

#include<iostream.h>   <<--- declaration of cout and cin

void main()  

{

    void fun();  <<--- function declaration

    cout<<"You are in main";

    fun(); <<--- function call

}

void fun()   <<--- function Definition

{

    cout<<"You are in fun";

}

```
## Declaration

1. Function declaration is also known as function prototype.

2. Function need to be declared before use(just like variable). 

3. Function can be declared locally or globally.

4. Return type function (argument list);

5. Function definition is a block of code.

## Formal and Actual Arguments
```cpp

#include<iostream.h>

int sum(int, int);

void main()

{

    int a = 5, b = 6;

    int s = sum(a, b); <<---  a and b are actual arguments
    
    cout<<"Sum is"<<s;


}

int sum(int x, int y)  <<--- x and y are formal arguments

{ 
    
    return (x + y);

}

```

## Inline Function

1. To eliminate the cost of calls to small functions, C++ proposes a new features called inline functions.

2. An inline functions is  a functions that is expanded in line when it is invoked.

3. Compiler replaces the functions call with the corresponding function corresponding code.

4. inline is a request not a command.

5. The benefits of speed of inline functions reduces as the functions grows in size.

6. So the Compiler may ignore the request in some situations:

Function containing loops, switch, goto.

Function with recursion.

Containg static variables.


## Example of inline function:

```cpp

#include<iostream.h>

inline void fun();

void main()

{
     
    cout<<"You are in main";

    fun();  

}

void fun()

{

    cout<<"You are in fun";
}

```