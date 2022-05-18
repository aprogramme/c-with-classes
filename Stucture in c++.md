

# Structure in C++

1. Structure are user defined data types.

2. Using structures allows us to combine data of different types together.

Three important points:

1. Structure is collection of dissimilar elements.

2. Structure is a way to group variables.

3. Structure is used to create data type


## Value declare, initialize at the time of declaration and initialize after declaration

```cpp

#include<conic.h>

#include<iostream.h>

struct book
{
    int book id;
    char title[20];
    float price;
};

int main()
{
    book b1 = {100, c++ course, 450.0};
    book b2, b3;
    b2.bookid = 101;
    strcpy(b2.title, "C++ made easy");
    b2.price = 300.0;

    b3 = b2;
}
```
## Take input from user
```cpp
#include<conio.k>
#include<iostream.h>
struct book
{
   int book id;
   char title[20];
   float price;
};

void display(book);
book input();
int main()
{
    book b1;
    b1 = input();
    display(b1);a
}

void display(book b)
{
    cout<<"\n"b.bookid<<" "<<b.title<<" "<<b.price;
}

book input()
{
    cout<<"Enter bookid, title and price of book";
    cin>>b.bookid>>b.title>>b.price;
    return(b);
}



