## 题目背景
Score: 15.

## 题目描述
There is a large amount of historical weather data for CEMCity. Each day in the data is listed as either a day with sunshine or a day with precipitation. Jeremy is interested in finding the record for the most consecutive days with sunshine. Unfortunately, the data is incorrect for exactly one day, but Jeremy doesn't know which day this is.

Your job is to help Jeremy determine the maximum possible number of consecutive days with sunshine.

![](https://cdn.luogu.com.cn/upload/image_hosting/mirndz24.png)

## 输入格式
The first line of input contains a positive integer, $N$, representing the number of days in the historical data. The following $N$ lines each contain either the character $S$ or the character $P$, representing a day with sunshine or a day with precipitation, respectively, in chronological order.

## 输出格式
Output the non-negative integer, $M$, which is the maximum possible number of consecutive days with sunshine.

```input1
8
P
S
P
S
S
P
P
S
```

```output1
4
```

## 提示
**Explanation of Output for Sample Input**

If the data is incorrect for the third day, then there was sunshine from the second day to the fifth day which is four consecutive days with sunshine. This is the maximum possible number of consecutive days with sunshine. That is, no matter which day the data is incorrect for, there were not five (or more) consecutive days of sunshine.

The following table shows how the available 15 marks are distributed:

|Marks|Description|Bounds|
|:-:|:-:|:-:|
|2|There are not many days in the historical data. The data consists of a single block of all S's followed by a single block of all P's. One of these blocks may be empty.|$N\leq 1000$|
|4|There are not many days in the historical data. The data contains S's and P's possibly in mixed order.|$N\leq 1000$|
|9|There are possibly many days in the historical data.|$N\leq 500\,000$|

