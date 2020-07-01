<center>
    c notebook
    <br>
    pzc
</center>
***

## 关键字

***

***

static:

1.隐藏全局变量，使变量对其他文件不可见

2.保持临时变量不被删除，控制使用范围

3.类中的静态函数与类无关，无需生成类即可使用，相当于命名空间下的函数

***

enum：

枚举成员，默认第一个数值为整型的0，后续每个数值+1，可在第任意个元素赋值（只影响后方元素）

不连续的枚举无法遍历

[1](https://www.runoob.com/cprogramming/c-enum.html)

***

void:

1.对函数返回的限定

2.对函数参数的限定   $int\ func(void)$ 不允许接受参数

3.void指针可以指向任意类型的数据

4.void（变量）告诉编译器变量已经使用，防止报警

***

this

const类型，永远指向当前所使用的类

***

inline

解决频繁调用小函数导致大量消耗栈空间的问题

必须与函数主体写在一起

不适用于函数体较长的情况

[1](https://www.runoob.com/w3cnote/cpp-inline-usage.html)

***

assert

断言，如果条件错误，终止程序

***

size_t

64位中为long long unsigned int, 非64位中为long unsigned int

***

## 特殊使用

***

***

nL:

表示长整型的n