# Mehtod overloading:
1.  Method overloading:
C++ allows specification of more than one function of the same name in the same scope. These functions are called overloaded functions. Overloaded functions enable you to supply different semantics for a function, depending on the types and number of arguments.11-Nov-2021

2. Mehtod Hiding:
This process is referred to as name hiding. In a member function definition, the declaration of a local name hides the declaration of a member of the class with the same name. The declaration of a member in a derived class hides the declaration of a member of a base class of the same name.

# Example:
```cpp
#include<conio.h>
#inlcude<iostream.h>
class A 
{
  public:
    void f1() { }
    void f2() { }
};
class B: public A 
{
  void f1() { }  //  method overloading
  void f2(int x) { }  // method hiding
};
void main()
{
  B obj;
  obj.f1();  // B
  obj.f2();  // error
  obj.f2(4)  // B
  getch();
}

