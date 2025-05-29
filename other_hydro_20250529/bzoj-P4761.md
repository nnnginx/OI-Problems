## 题目描述

Bessie has gotten herself stuck on the wrong side of Farmer John's barn again, and since her vision is so poor, she needs your help navigating across the barn.

The barn is described by an $n \times n$ grid of square cells, some being empty and some containing impassable haybales. Bessie starts in the lower-left corner (cell $1,1$) and wants to move to the upper-right corner (cell $n,n$). You can guide her by telling her a sequence of instructions, each of which is either "forward", "turn left $90$ degrees", or "turn right $90$ degrees". You want to issue the shortest sequence of instructions that will guide her to her destination. If you instruct Bessie to move off the grid (i.e., into the barn wall) or into a haybale, she will not move and will skip to the next command in your sequence.

Unfortunately, Bessie doesn't know if she starts out facing up (towards cell $1,2$ ) or right (towards cell $2,1$ ). You need to give the shortest sequence of directions that will guide her to the goal regardless of which case is true. Once she reaches the goal she will ignore further commands.



## 输入格式


The first line of input contains $n$.

Each of the $n$ following lines contains a string of exactly $n$ characters, representing the barn. The first character of the last line is cell $1,1$. The last character of the first line is cell $n,n$.

Each character will either be an `H` to represent a haybale or an `E` to represent an empty square.

It is guaranteed that cells $1,1$ and $n,n$ will be empty, and furthermore it is guaranteed that there is a path of empty squares from cell $1,1$ to cell $n, n$.



## 输出格式



On a single line of output, output the length of the shortest sequence of directions that will guide Bessie to the goal, irrespective whether she starts facing up or right.





```input1
3
EHE
EEE
EEE
```
```output1
9
```

## 数据规模与约定

对于 $100\%$ 的数据，$2 \leq n \leq 20$。