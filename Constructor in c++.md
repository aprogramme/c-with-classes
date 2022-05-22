# Constructor:
1. Constructor is a member function of a  class.
2. The name of the Constructor is same  as the name of the class.
3. It has no return type, so can't use return keyword.
4. It must be an instance member function, that is, it can never be static.

 # Example:
```cpp
#include<conio.h>
#include<iostream.h>
class complex
{
    private:
      int a, b;
    public:
      complex()
     {     }
};
```
# How to call constructor?
1. Constructor is implicity invoked when an object is created.
```cpp
 #incldue<conio.h>
 #include<iostream.h>
 class complex
 {
     private:
       int a, b;
     public:
       complex()
       { cout<<"Hello Contructor";}
 };

 void main()
 {
     clrscr();
     complex c1, c2, c3;
     getch();
 }
 ```

 2. Constructor is used to solve problem of initialization.
 3. What is problem of initialization?
   
  - When object are created, the members of the object cannot be initialized directly and this problem of not being able to initialize data members.
    
    
# Constructor Overloading
```cpp
#incldue<conio.h>
class complex
{
    private:
      int a, b;
    public:
      
      Complex(int x, int y)      // Parameterized Constructor
      { a = x; b = y; }

      Complex(int k)      // Parameterized Constructor
      { a = k; }
      Complex()   // default Constructor
      { }
};

void main()
{
    clrscr();
    Complex c1(3,4), c2;
    getch();
}
```

# Copy Constructor
```cpp
#incldue<conio.h>
class complex
{
    private:
      int a, b;
    public:
      
      Complex(int x, int y)      // Parameterized Constructor
      { a = x; b = y; }

      Complex(int k)      // Parameterized Constructor
      { a = k; }
      Complex()   // default Constructor
      { }
      Complex(Complex &c)
      {
          a = c.a;
          b = c.b;
      }
};

void main()
{
    clrscr();
    Complex c1(3,4), c2, c3(5);
    Complex c4(c1);
    getch();
}
```