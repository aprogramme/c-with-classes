# Abstract class in C++:
- Pure virtual function:

A do nothing function is pure virtual function.
```cppp
#include<conio.h>
#inlcude<iostream.h>
class Person
{
  public:
    virtual void fun() = 0;   // Pure Virtual function
    void f1()
    {  }
};
class Student : public Person
{ 
  public:
   void fun()
   {
     
   }
};
```
- A class containing pure virtual function is an abstract class.
- We can not instantiate abstract class.
# Why abstract class?
- An abstract class is used if you want to provide a common, implemented functionality among all the implementations of the component. Abstract classes will allow you to partially implement your class, whereas interfaces would have no implementation for any members whatsoever.
