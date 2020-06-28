> Class Memory:
>
> 模板T
>
> 继承标准库数据结构vector<T>
>
> resize：输入size和name，调用vector的resize（size）
>
> resize_min：输入size和name，判断当前size是否小于输入size，如果是则调用resize
>
> check_index： 输入index([Integer类型](../Math/Integer_h.md]))， 判断输入的index是否小于size
>
> capacity_in_bytes: 返回当前容量*T类型所需空间量，即总比特数

***

update 2020.6.28