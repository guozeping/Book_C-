<center><font size=50>const 成员函数</font></center>

# 一、const 成员函数

> const 成员函数可以使用类中的所有成员变量，但是不能修改它们的值，这种措施主要还是
>
> ***<font color=red>注意：</font>***
>
> 1、函数开头的 const 用来修饰函数的返回值，表示返回值是 const 类型，也就是不能被修改，例如`const char * getname()
>
> 2、函数头部的结尾加上 const 表示常成员函数，这种函数只能读取成员变量的值，而不能修改成员变量的值，例如`char * getname() const`