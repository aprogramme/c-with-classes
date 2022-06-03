# Function Overloading:
1. Function overloading is a feature of object oriented programming where two or more functions can have the same name but different parameters.

2. When a function name is overloaded with different jobs it is called Function Overloading.

3. In Function Overloading “Function” name should be the same and the arguments should be different.

4. Function overloading can be considered as an example of polymorphism feature in C++.

# Program:

#include <iostream>
```cpp
using namespace std;
int sum(int a, int b)
{
    cout<<"Using function with 2 arguments"<<endl;
    return a+b;
}

int sum(int a, int b, int c)
{
    cout<<"Using function with 3 arguments"<<endl;
    return a+b+c;
}
// calculate the volume of cylinder
int volume(double r, int h)
{
    return(3.14 * r * r * h);
}

// calculate the volume of cube
int volume(int a)
{
    return (a * a * a);
}

// calculate the volume of rectangular box
int volume(int l, int b, int h)
{
    return (l*b*h);
}

int main()
{
    cout<<"The sum of 3 and 6, "<<sum(3,6)<<endl;
    cout<<"The sum of 3, 7 and 6, "<<sum(3,7,6)<<endl;
    cout<<"The volume of cuboid of 3, 7 and 6 is "<<volume(3, 7,6)<<endl;
    cout<<"The volume of cylinder of redius 3 and height 6 is "<<volume(3, 6)<<endl;
    cout<<"The volume of cube of side 3 is "<<volume(3)<<endl;
    return 0;
}
```