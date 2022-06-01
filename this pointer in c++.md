# this pointer in c++:
- Object oriented:
A pointer contains address of an object is called object pointer.
```cpp
#inlcude<iostream.h>
Class Box
{
    private:
      int l, b, h;
    public:
      void setDimension(int x, int y, int z)
      { l = x; b = y; c = z}
      void showDimension()
      {
          cout<<"\nl="<<l<<"b="<<b<<"h="<<h;
      }
} 
void main()
{
    clrscr();
    Box *p, smallBox;
    p = &smallBox;

    p -> setDimension(12, 10, 5);
    p -> showDimension();
    getch();
}
```
- this pointer:
1. this is a keyword.
2. this is a local object pointer in every instance member function containing address of th caller object.
3. this pointer can not be modify.
4. It is used to refer caller object in member function.
 
 ```cpp
 #include<iostream.h>
 {
     private: 
       int l, b, h;
    public:
       void setDimension(int l, int b, int h)
       { this -> l = l; b = b; h = h}
      void showDimension();
      {
         cout<<"\nl="<<l<<"b="<<b<<"h="<<h;
      }
 };
 void main()
 {
     clrscr();
     Box smallBox;
     smallBox.setDimension(12,10,5);
     smallBox.showDimension();
     getch();
 }
