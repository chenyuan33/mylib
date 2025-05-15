# mylib

[English](README.md) | [中文](README_zh.md)

C++ 标准库的重制版。

## 关于

这个库是活跃的，接受 Issues 和 Pull Requests。

**但是**，这个库还没有完成。它会经常更新。目前，它只包含以下组件（只支持 C++98）：

- 无

## 如何使用

首先，使用 `git` 克隆仓库：

``` bash
git clone https://github.com/chenyuan33/mylib.git
```

然后，将 `include` 目录复制到你的项目目录，并将其重命名为 `mylib`。

然后，仓库的目录树应该如下所示：

``` plain
.
├── mylib
|   ├── algorithm
|   ├── array
|   ├── bitset
|   ├── ...
├── main.cpp /* Your code here */
```

包含头文件的方式如下：

``` cpp
#include "mylib/algorithm"
// 这将会等同于：
#include <algorithm>
```

然后，你可以在头文件中使用函数。例如：

``` cpp
#include "mylib/iostream"

int main() {
	mylib::cout << "Hello, mylib!" << mylib::endl;
	return 0;
}

**注意**，要使用库，你需要使用命名空间 `mylib`，而不是 `std`。
