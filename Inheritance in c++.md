# Inheritance in C++:
- Basic:
1. Class is used to describe properties ans behaviour of an object.
2. Property name and values.
3. Behaviour means actions.

- INHERITANCE:
1. It is a process of Inheriting properties and behaviour of existing class into a new class.
2. Existing class = old class = Parent class = Base class.
3. New class = child class = Derived class.

- SYNTAX: 
```cpp
{


};
class Derived_class : Visibility_Mode Base_class
{

};
```
- EXAMPLE:
```cpp
class car
{

};
class Sports car : public car
{

};
```

- TYPES OF INHERITANCE:
1. Single Inheritance
```cpp
class A
{

};
class B:public A
{

};
```
2. Multilevel Inheritance
```cpp
class A
{

};
class B:public A
{

};
class C:public B
{

};
```
3. MUltiple Inheritance
```cpp
class A1
{

};
class A2
{

};
class B:public A1, public A2
{

};
```
4. Hierarchical Inheritance
```cpp
class A
{

};
class B1:public A
{

};
class B2:public A 
{

};
```
5. HYbrid Inheritance



- Visibility Mode:
1. Private
2. Protected
3. Public

```cpp
#include<conio.h>
#include<iostream.h>
Class a
{
  private:
    int a;
  protected:
    void setValue(int k);
    { a = k; }
};
class B : public a
{
  public:
    void setData(int x)
    { setvalue(x); }
};
void main()
{
  B obj;
  obj.setData(4);
}
```

# Is-a relationship:
1. Relationship between two classes is called Association.
2. Types of association:
- Aggregation
- Composition
- Inheritance
EXAMPLE:

- Banana is a fruit

In this example banana is a child class and fruit is a parent class.

- Rectangle is a quadrilateral

Rectangle is a child class and quadrilateral is a parent class.

# Public Inheritance 
1. Is a relationship is always impliment as a public inheritance.
- Example:
```cpp
#inlcude<conio.h>
#inlcude<iostream.h>
class car
{
  private:
    int gear;
  public:
    void incrementGear()
    {
      if(gear<5)
      gear++;
    }
};
classSportsCar:public car
{

};

