# Friend Function:
1. Friend function is not a member function of a class to which it is a friend.
2. Frined function is declared in the class with friend keyword.
3. It must be defined outside the class to which it is friend.
4. Friend function can access any member of the class to which it is friend.
5. Friend function cannot access members of the class directly.
6. It has no caller object.
7. it should not be defined with membership label.

# Program:
```cpp
#include<conio.h>
#include<iostream.h>
Class Complex
{
  private:
    int a, b;
  public:
    void setData(int x, int y)
    { a = x; b = y; }
    void showData()
    { cout<<"a="<<a<<"b="<<b; }
    friend void fun(Complex);
};

void fun(Complex c)
{
  cout<<"sum is"<<c.a + c.b;
}
void main()
{
  clrscr();
  Complex c1, c2, c3;
  c1.setData();
  fun(c1);
  getch();
}

```
- - FRIEND FUNCTION CAN BECOME FRIEND TO MORE THAN ONE CLASS:
```cpp
#include<conio.h>
#include<iostream.h>
class B;
Class A;
{
  private:
    int a;
  public:
  void setData(int x) (a = x)
  friend void fun(A,B);
};

Class B;
{
  private:
    int b;
  public:
  void setData(int y) (b = y)
  friend void fun(A,B);
};

void fun(A o1, B o2)
{
  cout<<"sum if"<<o1.a + o2.b;
}
void main()
{
  clrscr();
  A obj1;
  B obj2;
  obj1.setData(2);
  obj2.setData(3);
  fun(obj1, obj2);
}
```

- - OVERLOADING OF OPERATORS AS A FRIEND FUNCTION:
```CPP
#inlcude<conio.h>
#inlcude<iostream.h>
Class Complex
{
private:
  int a, b;
public:
  void setData(int x, int y)
  { a = x; b = y; }
  void showData()
  {cout<<\na = "<<"b = "<<b;}
  friend Complex operator +(Complex, Complex);
};
Complex operator +(Complex X, Complex Y)
{
  Complex temp;
  temp.a = X.a + Y.a;
  temp.b = X.b + Y.b;
  return(temp);
}
void main()
{
  clrscr();
  Complex c1, c2, c3;
  c1.setData(3,4);
  c2.setData(5,6);
  c3 = c1 + c2;   //c3 = operator+(c1+c2);
  c3.showData();
  getch();
}
```
- - OVERLOADING OF URINARY OPERATORS AS A FREIND FUNCTION:
```cpp
#include<iostream.h>
#include<conio.h>
Class Complex
{
   private:
     int a, b;
   public:
     void setData(int x, int y)
     { a=x; b=y; }
    void showData()
      { cout<<"\na="<<a<<"b"<<b; }
      friend Complex operator-(complex);
};
Complex operator-(complex X)
{
  Complex temp;
  temp.a = -X.a;
  temp.b = -X.b;
  return(temp);
}
void main()
{
  clrscr();
  Complex c1, c2;
  c1.setData(3,4);
  c2 = -c1;       // c2 = operator -(c1)
  c2.showData();
  getch();
}
```

