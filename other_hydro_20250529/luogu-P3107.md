## 题目描述
Farmer John's cows are on a road trip!  The odometer on their car displays an integer mileage value, starting at X (100 <= X <= 10^18) miles at the beginning of their trip and ending at Y (X <= Y <= 10^18) miles at the end of their trip.  Whenever the odometer displays an 'interesting' number (including at the start and end of the trip) the cows will moo.  A number is 'interesting' if when you look at all its digits except for leading zeros, at least half of these should be the same.  For example, the numbers 3223 and 110 are interesting, while the numbers 97791 and 123 are not.

Help FJ count how many times the cows will moo during the trip.

## 输入格式
\* Line 1: The first line will contain two integers, X and Y, separated by a space.


## 输出格式
\* Line 1: A single integer containing how many times the cows will moo during the trip.


## 题目大意
农民约翰的牛正开始一个美妙的旅程。牛车的里程表上显示一个整数表示里程，旅程开始时里程数为 $X(100\le X\le 10^{18})$，结束时里程数为 $Y(X\le Y\le 10^{18})$。每当里程表显示一个有趣的数时（包括起点和终点数），牛们会发出愉快的叫声。


对于一个里程数的每一位，如果有至少一半的数字时相同的，则这个里程数一个有趣的数。例如：$3223$ 和 $110$ 是有趣的数，而 $97791$ 和 $123$ 则不是。

请计算，整个旅程中，牛们会发出多少吃愉快的叫声。


```input1
110 133 

```

```output1
14 

```

## 提示
The trip starts with the odometer at 110 and ends at 133. 

The cows moo when the odometer reads 110, 111, 112, 113, 114, 115, 116, 117, 118, 119, 121, 122, 131, and 133. 



