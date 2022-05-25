# Operator Overloading:

1. when an Operator is overloading with multiple jobs, it is known as Operator overloading.

2. It is a way to impliment compile time polymorphism.

# Program:
```cpp
#include <iostream>
#include<conio.h>

class Complex
{
    private:
     int a, b;
    public:
     void setData(int x, int y)
     { a = x; b = y; }
     void showData()
     { cout <<\na = "<<a<<"b = "<<b"; }
     Complex add(Complex c)
     {
         Complex temp;
         temp.a = a + c.a;
         temp.b = b + c.b;
         return (temp);
     }
};

void main()
{
    clrscr();
    Complex c1, c2, c3;
    c1.setData(3, 4);
    c2.setData(5, 6);
    c3 = c1.add(c2);
    c3.showData();
    getch();
}
```
# Rules to Remember:
- Any symbol can be used as function name if it is a valid operator in c language.

- We can not overload sizeof and ?: operator.

- We can't use other symbol except alphabet, digit and underscore as a function name.

 - If we use a operator symbol as a function name then must use 'operator' keyword before symbol.

 - We use only those operator symbol as a function name which was a valid opertaor in C.

# Program:
```cpp
#include<conio.h>
#include<oistream.h>
class Complex
{
    private:
      int a, b;
    public:
      void setData(int x, int y)
      { a = x; b = y; }
      void showData()
      { cout<<a =" <<a<<" b = "<<b;}
      Complex operator+(complex c)
      {
          Complex temp;
          temp.a = a + c.a;
          temp.b = b + c.b;
          return (temp);
      }
};

void maib()
{
    clrscr();
    c1.setData(3, 4);
    c2.setData(5, 6);
    c3 = c1 + c2;
    c3.showData();
    getch();
}
```
# Overloading of urinary operator:
```cpp
#include<conio.h>
#include<oistream.h>
class Complex
{
    private:
      int a, b;
    public:
      void setData(int x, int y)
      { a = x; b = y; }
      void showData()
      { cout<<a =" <<a<<" b = "<<b;}
      Complex operator-()
      {
          Complex temp;
          temp.a = -a;
          temp.b = -b;
          return(temp);
      }
};
void main()
{
    clrscr();
    Complex c1, c2;
    c1.setData(3,4);
    c2=c1.operator-();
    c2.showData();
    getch();
}
```
- Left operand in binary operarion is collor object.
  
  c3 = c1+c2  -------> c1 is collor object

- There are only one collor object in urinary operator.

# Overloading of Increment operator

1. Preincrement operator(++a)
2. Postincrement operator(a++)

```cpp
#include<conio.h>
#include<iostream.h>
class Integer
{
    private:
      int x;
    public:
      void setData(int a)
      { x = a; }
      void showData()
      { cout<<"x"<<x: }
      Integer operator++() // preincrement
      {
          Interger i;
          i.x = ++x;
          return(i);
      }
      Interger operator++(int) // post increment
      {
          Interger i;
          i.x = x++;
          return(i);
      }

};
void maiN()
{
    clrscr();
    Interger i1, i2;
    i1.setData(3);
    i1.showData();
    i2 = ++i1;   // i2 = i1.operator++();
    i1.showData();
    i2.showData();    
    getch();
}