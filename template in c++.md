# Template in C++:
1. The keyword template is used to define function template and class template.
2. It is way ti make your function or class generalize as fas as data type is concern.
- FUNCTION TEMPLATE:
```cpp
#include <iostream>

using namespace std;

    template <class X>
    X big(X a, X b)
    {
        if(a>b)
        return(a);
        else
        return(b);
    }

int main()
{
    cout<<big(4,5);
    cout<<big(5.6,3.4);
    

    return 0;
}
```
- CLASS TEMPLATE:
```cpp
#include <iostream>
using namespace std;

// Class template
template <class T>
class Number {
   private:
    // Variable of type T
    T num;

   public:
    Number(T n) : num(n) {}   // constructor

    T getNum() {
        return num;
    }
};

int main() {

    // create object with int type
    Number<int> numberInt(7);

    // create object with double type
    Number<double> numberDouble(7.7);

    cout << "int Number = " << numberInt.getNum() << endl;
    cout << "double Number = " << numberDouble.getNum() << endl;

    return 0;
}
```