# mylib

[English](README.md) | [中文](README_zh.md)

A remake of the C++ standard library.

## About it

This library is active and welcome issues and pull requests.

**But** this library is not complete yet. It will be updated frequently. Currently, it only includes the following components (only C++98):

- None

## How to use

First, using `git` to clone the repository:

``` bash
git clone https://github.com/chenyuan33/mylib.git
```

Then, you need to copy the directory `include` to your project directory and rename it to `mylib`.

Then, the tree of the repository should look like this:

``` plain
.
├── mylib
|   ├── algorithm
|   ├── array
|   ├── bitset
|   ├── ...
├── main.cpp /* Your code here */
```

You can include the header files in your code like this:

``` cpp
#include "mylib/algorithm"
// It is same as that:
#include <algorithm>
```

And then, you can use the functions in the header files. For example:

``` cpp
#include "mylib/iostream"

int main() {
    mylib::cout << "Hello, mylib!" << mylib::endl;
    return 0;
}
```

**Note** that to using the library, you need to using the namespace `mylib` but not `std`.
