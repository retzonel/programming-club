## learning about const and namespaces
```cpp
#include <iostream>

int main()
{
    const double pi = 3.14;
    double radius = 10;
    double circumfrence = 2 * pi * radius;

    std::cout << circumfrence << "cm";

    // const adds data security,
    // they cant be reassigned a new value
    //const == "make readonly after decleration" 
    return 0;
}
```

```cpp
#include <iostream>

namespace first
{
    int x = 1;
}

namespace second
{
    int x = 2;
}

int main()
{
    using std::cout;
    // namespace prevents name conflicts
    /*
    two vairables can be the same name without errors
    if they are in different namespaces
    */
   using namespace second;
   std::cout << first::x << "\n";
   std::cout << x;

   //:: referes to the scope resoluton operator
   //using namepace std???
   

    return 0;
}



```
