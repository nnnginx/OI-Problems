## 题目描述

万老板希望在新的智能音乐播放设备IPOOD中，实现对波文件音质性能的评定。离散的波文件被考虑为长度为 N 的整数序列：Al,A2,...,AN。所谓的音质性能检测，可以评定任何的一个区间范围 [L,R] ，音质性能取决于下述评分：

![](./3635/file/pic1.png)

其中 F 是可归纳定义的数列，满足 F[1]=1，F[2]=2 且 F[k+2]=F[k+1]+aF[k]+b 对于任何 k>=l 成立。其中 a 和 b 为正整系数。为了可以为用户提供更好的服务体验，并希望对给定的波文件进行修正优化。这一款设备中，还应该支持对波文件的修改。对于给定的区间范围 [L,R] ，允许用户将 A[L] 至 A[R] 同时增加一，或同时减少一。

## 输入格式
输入的第一行有两个正整数，波文件的总长度 N ，和总的修改与询问次数 Q 。

第二行有两个整数，分别表示系数 a 和 b 。

之后若干行，一共给出 N 个正整数 A1 到 AN ，满足 1≤A[i]≤2*109 。

之后 Q 行，每行是下述三种形式之一：
- plus L R：将波文件数列中下标在区间 [L,R] 内的元素每一个都加一。
- minus L R：将波文件数列中下标在区间 [L,R] 内的元素每一个都减一。
- query L R：询问区间 [L,R] 的音质性能评分。

修改和询问中，均保证 L≤R ，且保证 A[i] 严格大于总的修改次数加一(修改操作包括 plus 和 minus 两种)。
N≤300000，Q≤10000，0≤a,b≤10^9
## 输出格式
 输出若干行，每一行对应一次询问，输出一个整数。

```input1
7 7 
1 0 
3 4 5 6 7 8 9 
query 2 4 
query 3 7 
plus 3 5 
query 2 4 
plus 4 7 
query 3 7 
query 1 7

```

```output1
64 
1766 
104 
7479 
7687
```

## 提示
没有写明提示
## 题目来源
没有写明来源


