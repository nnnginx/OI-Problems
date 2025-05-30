## 题目描述
Some major cities have subway systems in the form of a tree, i.e. between any pair of stations, there is one and only one way of going by subway. Moreover, most of these cities have a unique central station. Imagine you are a tourist in one of these cities and you want to explore all of the subway system. You start at the central station and pick a subway line at random and jump aboard the subway car. Every time you arrive at a station, you pick one of the subway lines you have not yet travelled on. If there is none left to explore at your current station, you take the subway line back on which you first came to the station, until you eventually have travelled along all of the lines twice,once for each direction. At that point you are back at the central station. Afterwards, all you remember of the order of your exploration is whether you went further away from the central station or back towards it at any given time, i.e. you could encode your tour as a binary string, where 0 encodes taking a subway line getting you one station further away from the central station, and 1 encodes getting you one station closer to the central station.

![](https://cdn.luogu.com.cn/upload/image_hosting/57sf9gvq.png)

## 输入格式
On the first line of input is a single positive integer n, telling the number of test scenarios to follow.Each test scenario consists of two lines, each containing a string of the characters '0' and '1' of length at most 3000, both describing a correct exploration tour of a subway tree system.

## 输出格式
exploration tours of the same subway tree system, or the text "different" if the two strings cannot be exploration tours of the same subway tree system.

## 题目大意
**【题目描述】**

一些主要城市的地铁系统采用树状结构，即在任何两个车站之间，只有一条且仅有一条地铁线路。此外，大多数这些城市都有一个独特的中央车站。想象一下，你是这些城市中的一名游客，你想要探索整个地铁系统。你从中央车站出发，随机选择一条地铁线路，跳上地铁列车。每当你到达一个车站，你就会选择一条你尚未乘坐过的地铁线路。如果在当前车站没有其他要探索的地铁线路了，你就会乘坐第一次到达该车站的地铁线路返回，直到最终你沿着所有的线路都行驶了两次，即每个方向都行驶了一次。在那时，你回到了中央车站。之后，你所记得的探索顺序只是在任何给定时间是否向中央车站更远或更近，也就是说，你可以将你的旅程编码为一个二进制字符串，其中 0 表示乘坐一条地铁线路使你离中央车站更远一站，而 1 表示使你离中央车站更近一站。

**【输入格式】**

输入的第一行是一个正整数 $n$，表示接下来要跟随的测试方案的数量。每个测试方案包括两行，每行包含一个长度最多为 $3000$ 的由字符 '0' 和 '1' 组成的字符串，描述了地铁树系统的正确探索旅程。

**【输出格式】**

对于每个测试方案，如果两个字符串可以表示相同地铁树系统的探索旅程，则输出 "same"；如果两个字符串不能表示相同地铁树系统的探索旅程，则输出 "different"。

翻译来自于：ChatGPT。

```input1
2
0010011101001011
0100011011001011
0100101100100111
0011000111010101
```

```output1
same
different
```

