整数的类别实现：

>Class IntBase
>
>模板T
>
>变量
>
>T类变量a
>
>N_BYTES：T所占空间
>
>N_BITS: 8个T所占空间
>
>MAX_N_BITS：即N_BITS，所在总空间量
>
>函数：
>
>size：返回T所占空间量
>
>length：返回总空间量，即8个T所占空间量
>
>type_string：返回"Integer"
>
>allows：输入[Dtype 类型](field_types_h.md)，返回其是否小于或等于[DATA_BIT](field_types_h.md)
>
>构造函数：接受输入a，默认a为0
>
>get：返回a的值
>
>get_bit: 输入i，返回a二进制下右边第i位的值
>
>get_ptr: 返回指向a的指针
>
>debug: 返回a
>
>assign: 输入长整型或者无类型指针。如果是长整型x则将x赋值给a，如果是无类型指针则从其所指向的空间去sizeof(a)个bit赋值给a
>
>assign_zero：a=0
>
>assign_one: a=1
>
>is_zero: 返回a==0
>
>is_one: 返回a==1
>
>is_bit：返回a==1或a==0
>
>



***

update 2020.6.27