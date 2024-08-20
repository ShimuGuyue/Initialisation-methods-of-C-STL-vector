vector 使用方法：

```c++
std::vector<数据类型T> 容器名(int 容器大小 = 0, 数据类型T 数据元素 = NULL);
```

一维数组用法：

```c++
// 创建一个 vector 容器 a1，数据类型为 int，大小为 0，无数据元素
std::vector<int> a1;
// null

// 创建一个 vector 容器 a2，数据类型为 int，大小为 n2，数据元素初始化默认为 0
int n2(2);
std::vector<int> a2(n2);
// 0 0

// 创建一个 vector 容器 a3，数据类型为 int，大小为 n3，数据元素初始化为 k3
int n3(2);
int k3(5);
std::vector<int> a3(n3, k3);
// 5 5
```

多维数组用法（二维数组举例）：

```c++
// 创建一个 vector 容器 a4，数据类型为 vector<int> 容器，大小为 0，无数据元素
std::vector<std::vector<int>> a4;
// null

// 创建一个 vector 容器 a5，数据类型为 vector<int> 容器，大小为 n5，
// 数据元素初始化默认为大小为 0，无数据元素的 vector<int>【和 a1 一样】
int n5(2);
std::vector<std::vector<int>> a5(n5);
// null
// null

// 创建一个 vector 容器 a6，数据类型为 vector<int> 容器，大小为 n6，
// 数据元素初始化默认为大小为 m6，数据元素初始化默认为 0 的 vector<int>
int n6(2);
int m6(3);
std::vector<std::vector<int>> a6(n6, std::vector<int>(m6));
// 0 0 0
// 0 0 0

// 创建一个 vector 容器 a7，数据类型为 vector<int> 容器，大小为 n7，
// 数据元素初始化默认为大小为 m7，数据元素初始化默认为 k7 的 vector<int>
int n7(2);
int m7(3);
int k7(5);
std::vector<std::vector<int>> a7(n7, std::vector<int>(m7, k7));
// 5 5 5
// 5 5 5
```

------

转载请附链接[Upload files · ShimuGuyue/Initialisation-methods-of-C-STL-vector (github.com)](https://github.com/ShimuGuyue/Initialisation-methods-of-C-STL-vector)

知识需要得到传播，

但绝不能因此成为某些人捞黑钱的手段！！！