<center>
    leetcode notebook
    <br>
    pzc
</center>
***

滑动窗口：

使用情景：

用于寻找某个连续的子集

方法：

初始化左右指针，根据不同的判断向同方向移动，指导遍历整个集合

例子：

[无重复字符的最长子串](https://leetcode-cn.com/problems/longest-substring-without-repeating-characters/)

***

二分查找：

使用情景：

在有一定顺序的数中找到某个特定的数，且要求的时间复杂度为$O(logn)$

方法：

每次查找排除掉一半的元素，再继续下一次查找

例子：

[寻找两个正序数组的中位数](https://leetcode-cn.com/problems/median-of-two-sorted-arrays/)

***

数组划分：

使用情景：

需要将数组分为几个部分，如寻找某个特定值或拆分数组，本质是找到数组中的某个特定值

方法：

例子：

[寻找两个正序数组的中位数](https://leetcode-cn.com/problems/median-of-two-sorted-arrays/)

***

动态规划：

使用情景：

问题可以用递归的形式分解，并且初始情况容易解得。类似与第一类和第二类数学归纳法。一般在只求某个较大值的时候效率较低，求多个值使用效果较好，需保存中间过程的值，内存开销较高。

方法：

通过递归使问题一步一步分解到简单情况，使用第二类数学归纳法则需要保存中间过程的结果

例子：

[最长回文子串](https://leetcode-cn.com/problems/longest-palindromic-substring/)

[正则表达式匹配](https://leetcode-cn.com/problems/regular-expression-matching/)

***

* Manacher算法：

[最长回文子串](https://leetcode-cn.com/problems/longest-palindromic-substring/)

在中心扩展的前提下加一个臂长length，被臂长已经覆盖过的位置无需再次计算，只需$O(n)$的空间复杂度。

只能找出最长的子串（臂长排除掉了较短的），不能找出所有子串。

***

确定有限自动状态机

特点：

1. 在DFA中，给定当前状态，我们能够知道下一个状态。
2. 下一个状态是唯一确定的。
3. 从符号空间中选择任意一个符号输入，总有一个唯一确定的下一状态。比如上图中，符号空间为{0，1}，当前状态为A，输入1，那么下一个状态百分之百是B，输入0，为C，其它状态亦然。
4. 简单且容易实现

***

非确定有限自动状态机

1. 在NFA中，给定当前状态，可能有多个下一个状态。
2. 可以随机选择下一个状态。
3. 可以并行（同时）选择下一个状态。
4. 输入符号可以为空。

***

双指针

使用情况：

找到数组中所要求的范围（类似滑动窗口）

用法：

初始化左右指针为边界（也可能是其他位置），根据当前情况不断缩小，直到找到要求的范围或者遍历完整个数组。移动时要有明确的判定，以确定移动左指针或右指针，不能明确决定的问题一般不可用。

例子：

[盛最多水的容器](https://leetcode-cn.com/problems/container-with-most-water/)（移动较小的指针）

[三数之和](https://leetcode-cn.com/problems/3sum/)（同时移动左右指针，左指针增大，右指针减小）

***

