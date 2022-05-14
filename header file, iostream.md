

# Header File

Predefined function are declared in header file, so whenever you are using any predefined function in your code, you have to include specific header file that contains it's declaration.









# iostream.h

1. we need to include header file iostream.h. it contains declaration for the identifier cout and the operator <<, and also for identifier cin and operator >>.
2. Header file contains declaration of identifier.
3. identifiers can be function names, variables, objects, macros, etc.
## endl

1. insertion endl into the output stream causes the screen cursor to move to the beginning of the next line.

2. endl is a manipulation and it is declared in iostream.h .
3. '\n' charactor also works as it works in c.




## Sample Program(square.cpp)
```cpp

#include<iostream.h>

#include<conic.h>

void main()

{

clrscr();

int x;

cout<<"Enter a number"<<endl;

cin>>x;
int s = x * x;

cout<<"Square of "<<x<<" is <<s;

getch();

}
```

