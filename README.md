### BigNumberCalculator 大数计算器

#### 实现思路

1. 大数计算部分
    + 利用vector来分别倒序储存整数位与小数位
    + 重载运算符
    + 对只能对整数进行的运算进行特判
    + 对符号进行特别处理
2. 栈计算器部分
    + 构造符号栈与数字栈
    + 判断运算符优先级，如果优先级高的话就进行出栈计算再入栈
    + 添加特殊符号来标识运算结束

#### 使用

`cmake -DCMAKE_BUILD_TYPE=Debug/Release`

**预生成ELF位于`\bin`下**