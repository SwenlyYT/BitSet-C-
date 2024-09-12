# BitSet-C-

#include "BitSet.h"

bitset<8> byte = bitset<8>("00000001");

std::cout << sizeof(byte) << '\n'; // 1

byte.set(1);
byte.set(2);

std::cout << byte.to_string() << '\n'; // 01100000

byte.reset(2);

std::cout << byte.to_string() << '\n'; // 01000000

byte.set(2);
byte.set(5);
byte.reset(0);

std::cout << byte.to_string() << '\n'; // 01100100
