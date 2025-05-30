## 题目背景

奶牛们开始对用射电望远镜扫描牧场外的宇宙感兴趣。最近，他们注意到了一种非常奇怪的脉冲调制微波从星系的中央发射出来。他们希望知道电波是否是被某些地外生命发射出来的，还是仅仅是普通的的星星发出的。 

## 题目描述

帮助奶牛们用一个能够分析他们在文件中记下的记录的工具来找到真相。他们在寻找长度在 A 到 B 之间（包含 A 和 B 本身）在每天的数据文件中重复得最多的比特序列。他们在找那些重复得最多的比特序列。一个输入限制告诉你应输出多少频率最多的序列。  
符合的序列可能会重叠，并且至少出现一次的序列会被计数。  

## 输入格式

第一行： 三个用空格分隔的整数: A, B, N    
第二行及以后: 一个最多 $200000$ 字符的序列 S ，全是 $0$ 或 $1$ ， 并且每行字符数不大于 $80$ 。

## 输出格式

输出N个频率最高的序列（按照频率由高到低的次序）。由短到长排列频率相同的这些序列，如果长短相同，按二进制大小排列。如果出现的序列个数小于N，输出存在的序列。  
对于每个存在的频率，先输出单独包含该频率的一行，再输出以空格分隔的这些序列。每行六个（除非剩下的少于六个）。  

## 样例输入

```  
2 4 10  
01010010010001000111101100001010011001111000010010011110010000000  
```  

## 样例输出

```  
23  
00  
15  
01 10  
12  
100  
11  
11 000 001  
10  
010  
8  
0100  
7  
0010 1001  
6  
111 0000  
5  
011 110 1000  
4  
0001 0011 1100  
```

## 说明  
在样例里，序列 `100` 出现了 $12$ 次，而序列 `1000` 出现了 $5$ 次。次数最多的序列是 `00` ，出现了 $23$ 次。  

## 数据规模与约定

$1 \le N < 50$ , $1 \le A \le B \le 12$ , S 全部由 $0$ 或 $1$ 组成, 且长度不大于 $200000$ , 每行长度不大于 $80$

## 题目来源

题目翻译来自 NOCOW。  