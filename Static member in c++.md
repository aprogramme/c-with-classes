## Static Members in C++

1. Static local variables:

- Static variables are variable which have a property of preserving their values even when they go out of scope.
- Static variables remains in memory throughout the span of the program.
- Static variable are initialized to 0 if not initialized explicity.

# Example
```cpp
#include<conio.h>
#include<istream.h>
 void fun()
 {
     static int x;  // x is static local variable
     int y;  // y is not static local variable
 }

 ```

2. Static Member variable:
- Declared inside the class body.
- Also known as class member variable.
- They must be defined outsied the class.
- Static member variable does not belong to any object, but to the whole class.
- There will be only one copy of static member variable for the whole class
- Any object can use the same copy of class variable.

 
# Program
```cpp
#include<iostram.h>
#inlclude<conio.h>
clas Account
{
    private:
     int balance; // instance member variable
     static float roi; // Static member variabel/ Class variable
    public:
    void setBalance(int b)
    { balance = b;}
    static void setRoi(float r) // static Member fucntion
    { roi = r;}
};

float Account :: roi = 3.5f;
void main()
{
    clrscr();
    Account a1, a2;
    a1.setRoi(4.5f);
    Account::setRoi(4.5f);
}
```

- They are qualified with the keyword static.
- They are also called class member function.
- They can be invoked with or without object.
- They can only access static members of the class.


