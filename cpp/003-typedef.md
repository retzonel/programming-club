## type definitions

```cpp
#include <iostream>
#include <vector>

typedef std::vector<std::pair<std::string, int>> pairList_t;
typedef std::string text_t;

using text_nt = std::string;

int main()
{
    //type def gives niknames to data types
    //helps with code readability and reusablility
    //you can use the using keyword tho
   pairList_t pairList;
   text_t firstName = "Retzonel";

   std::cout << firstName;

    return 0;
}
```
