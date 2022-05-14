

# Default Arguments in C++

A default arguments is a value provided in a function declaration that is automataically assigned by the compiler if the caller of the function doesn't procide a value for the argument with a default value. In case any value is passed ithe default value is overridden.

## Default Arguments

```cpp

#include<conic.h>

#include<iostream.h>

int add(int, int, int = 0);

void main()

{

    int a, b;

    cout<<"Enter two numbers";

    cin>>a>>b;

    cout<<"Sum is"<<add(a,b);
    

    int c;

    cout<<"Enter three number";

    cin>>a>>b>>c;

    cout<<"Sum is"<<add(a,b,c);

    getch();
}

int add(int x, int y, int z)

{

    return (x+y+z);
}

```
## Function Overloading

When one function name overloaded with different hob it is known as function overloading.

POLYMORPHISM:

It means same things have multiple interpretation and each and every interpretation meaning will cleared in different  context.


There are 3 ways to impliment polymorphism:

1. Function overloading -> compile time polymorphism

2. Operator overloading -> compile time polymorphism

3. Virtual function -> Run-time polymorphism.

# Program
```cpp

#include<conic.h>

#include<iostream.h>

int area(int, int);

float area(int);

void main()

{

    int r;

    cout<<"Enter radius of circle";

    cin>>r;

    float A = area(r);

    cout<<"Area of circle is"<<A;

    int l, b, a;

    cout<<"Enter lenght and breadht of rectangle";

    cin>>l>>b;

    a = area(l, b);

    cout<<"Area of recangle is"<<a;

    getch();

}

float area (int R);

{

    return(3.14*R*R);

}

int area (int L, int R);

{

    return(L + B);
}

```
## How  function overloading is resolved?

1. First, c++ tries to find an exact match. This is the case where the actual argument exactly matches the parameter type of one of the overloading function.

2. If no exact match is found, C++ tries to find a match through promotion.

@ char, unsigned char and short is promoted to an int.

@ float is promoted to double.

3. If no promotion is found, C++ tries to find match through standard conversion.



