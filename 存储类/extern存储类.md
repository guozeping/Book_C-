<center><font size=50>extern 存储类</font></center>

# 一、extern存储类

> extern 存储类用于提供一个**全局变量**的引用，全局变量对所有的程序文件都是可见的。当您使用`extern`时，对于无法初始化的变量，会把变量名指向一个之前定义过的存储位置。
>
> 当您有多个文件且定义了一个可以在其他文件中使用的全局变量或函数时，可以在其他文件中使用extern来得到已定以的变量或函数的引用。可以这么理解，extern是用来在另一个文件中声明一个全局变量或函数。
>
> extern修饰符通常用于当有俩个货多个文件共享相同的全局变量或函数的时候，如下所示。

```c++
#include <iostream>
int count;
extern void write_extern();
int main()
{
  count = 5;
  write_extern();
}
```



