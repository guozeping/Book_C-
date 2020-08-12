<center><font size=50>const 对象</font></center>

# 一、const 对象

	> const也可以用来修饰对象，称为**常对象**。一旦将对象定义为常对象之后，就只能调用类的const 成员(包括const成员变量和const成员函数)了。

## 1.1 定义常对象

方法一：

```c++
const class object(params);
class const object(params);
```

方法二：定义const 指针

```c++
const class *p = new class(params);
class const *p = new class(params);
```

`class`为类名，`object`为对象名，`params`为实参列表，`p`为指针名。两种方式定义出来的对象都是常对象。

> ***<font color=red>注意：</font>***
>
> *一旦将对象定义为常对象之后，不管是哪种形式，该对象就只能访问被 const 修饰的成员了（包括 const 成员变量和 const 成员函数），因为非 const 成员可能会修改对象的数据（编译器也会这样假设），C++禁止这样做。*

