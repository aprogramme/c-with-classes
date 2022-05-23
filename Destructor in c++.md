# Destructor in C++:
1. Destructor is a instance member function of a class.
2. The name of the destructor is same as the name of a class preceded by tilde(~) symbol.
3. Destructor can never be static.
4. Destructor has no return type.
5. Destructor takes no arguments(No overloading is possible).


 # Example:
```cpp
#include<conio.h>
#include<iostream.h>
class Complex
{
    private:
     int a, b;
    public:
     ~Complex()
     { Cout<<"Destructor";}  
};

void fun:
{
    Complex obj;
}
void main()
{
    clrscr();
    fun();
    getch();
}
```
# Why Destructor?
it should be defined to release resources allocated to an object.

For example:

- Let's say there is an object of any class and there is a member variable (pointer) in an object.

- This pointer points the address some external memory(resource).

- If object get destroy, then pointer is also destroyed and we cant access the location of resource the pointer pointed.

- So we can't release memory of resource after destroyed of an object.

- In this situation we do a code in Destructor to release the memory of resource just before destroyed of an object.



