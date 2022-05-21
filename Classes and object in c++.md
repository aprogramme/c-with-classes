

# Classes and Object

The only dilfference between Structure and class is that,

1. the members of structures are by default public and

2. the members of class are by default private.

## Program
```cpp
#include<iostream.h>
#include<conio.h>
class complex()
{
    private:
      int a, b;
    public:
      void set_data(int x, int y)
      { a=x; y=b; }
      void show_data()
      {cout<<"\n a = " << a << " b = " << b;}
};

 void main()
 {
     clrscr();
     complex c1;    // c1 is an object
     c1.set_data(3, 4);
     c1.show_data();
     getch();
 }
```

# Complex Program

```cpp
#include<conio.h>
#inlcude<iostream.h>
class complex
{
    private:
      int a, b;
    public:
      void set_data(int x, int y)
      { a=x; y=b; }
      void show_data()
      {cout<<"\n a = " << a << " b = " << b;}
    complex add(complex c)
    {
        complex temp;
        temp.a = a + c.a;
        temp.b = b + c.b;
        return(temp);
    }
};

void main()
{
    clrscr();
    complex c1, c2, c3;
    c1.set_data(3, 4);
    c2.set_data(5, 6);
    c3 = c1.add(c2);
    c3.show_data();
    getch();
}
```
# Techical jargons

1. Class is a description of an object.
2. Object is an instance if a class.

  
  instance member variable
  - attribute, datamembers, field, properties

  instance member function
  - Method, procedure, actions, operation, services.

