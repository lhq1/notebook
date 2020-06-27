Bitvec_cpp为空，所有实现均在头文件中

Bitvec=Bitvec_<long>

>Class BitVec_
>
>模板T
>
>继承于[IntBase<T>](Integer_h.md)
>
>变量：
>
>n_bits: 8*T类所占用的空间量 
>
>函数：
>
>type_char： 返回'B'
>
>field_type： 返回DATA_GF2([DataFieldType类](field_type_h.md))
>
>allows： 输入dtype，返回dtype是否等于[DATA_TRIPLE](field_type_h.md)或者[DATA_BIT](field_type_h.md)
>
>构造函数：继承于[IntBase](Integer_h.md)，Z2<K>待处理
>
>运算符重载：
>
>+-：按位异或
>
>*：位与
>
>/：报错
>
>extend_bit: 最后一位是1则返回-1，否则返回0
>
>mask：输入整数n，返回a的右边n位
>
>add： 待处理
>
>randomize: 待处理
>
>pack： 待处理
>
>unpack： 待处理
>
>unpack_new： 待处理

***

update 2020.6.27