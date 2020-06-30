> class FixedVec
>
> 模板T，整数L
>
> v: array<T,L>
>
> length: L
>
> size: 返回L*T::size()
>
> typre_string: "T::type_string^L"
>
> type_short: T::type_char
>
> DataFieldType: 返回T:: field_type()
>
> Mul: 输入FixedVec a和某类数据b, 返回FixedVec res, res中每个元素为a中每个元素T::Mul(a[i],b)
>
> 构造函数：输入T类元素，v中每个元素等于输入，默认为0。输入FixedVec，复制。输入array，v=输入。
>
> get: 返回v
>
> negate: 所有元素取负
>
> assign:输入T类，使每个元素等于输入。输入指针buffer，将v中每个元素赋值为buffer所指内存相应位置的元素。
>
> assign_zero：全部赋值为0
>
> assign_one: 前部赋值为1
>
> equal：输入FixedVec，判断是否每个元素都相等
>
> is_zero: 判断是否所有元素为0
>
> is_one：判断是否所有元素为1
>
> sum: 返回v中所有元素和
>
> extend_bit: 返回FixedVec res，res中每个元素等于v中每个元素取extend_bit
>
> mask: 输入整型，返回FixedVec res，res中每个元素等于v中每个元素取mask（输入）
>
> randomize： 待处理
>
> almost_randomzie： 待处理
>
> randomize_to_sum： 待处理
>
> force_to_bit： 对v中每个元素取force_to_bit
>
> get_bit: 输入整型i，返回二进制右边第i位
>
> output: 输入ostream &s和bool human，对v中每个元素使用output(s,human)
>
> input： 输入istream &s和ool human，对v中每个元素使用input(s,human)
>
> pack：待处理
>
> unpack： 待处理

***

update 2020.6.30