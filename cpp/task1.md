### Retzonel

## Programming club Task 1

### Solutions to work problems

A nibble is 4 bits,  a byte is 8 bits, and a word is 12 bits. If the maximum amount of space given to a data type is 2 bytes and mega is the largest data type, then mega has: 
				2 * 1byte = 2 * 8bits
				= 16 bits

```cpp
#include <iostream>


namespace intNs
{
    int sum(int x, int y)
    {
        return x + y;
    }
}


namespace longNs
{
    long sum(long x, long y)
    {
        return x + y;
    }
}


int main()
{
    using std::cout;


    cout << longNs::sum(1, 3) << " long " << "\n";
    cout << intNs::sum(2, 6) << " int ";


    return 0;
}
```

Subtracting 1 from an unsigned int variable with a value of 0 will return (2^32) - 1 = 4294967296 - 5.
The min-max numbers an unsigned int can hold ranges from 0 - 4294967295, so when 0 - 1 executes the integer overflows (because there are not enough or too little bits to represent the unsigned int properly) and so it wraps.
The output is 429496725.
Integer overflow (unsigned overflow)

