## 题目描述

Farmer John's cows recently received a large piece of marble, which, unfortunately, has a number of imperfections. To describe these, we can represent the piece of marble by an $n$ by $ n$ square grid, where the character `*` represents an imperfection and `.` represents a flawless section of the marble. The cows want to carve a number  `8` in this piece of marble (cows are quite fond of the number `8` since they have cloven hooves on each of their four feet, so they can effectively count up to 8 using their "toes"). However, the cows need your help to determine the optimally placed figure eight in the piece of marble. Here are a few properties that define a valid figure eight:

* A figure eightconsists of two rectangles, a top and a bottom.
* Both the top and bottom have at least one cell in their interior.
* The bottom edge of the top rectangle is a (not necessarily proper) subset of the top edge of the bottom rectangle.
* The figure eight can only be carved from flawless regions of the piece of marble. The aesthetic score of a figure eight is equal to the product of the areas enclosed by its two rectangles. The cows wish to maximize this score. For example, given this piece of marble.

```plain
...............

...............

...*******.....

.*....*.......*

.*......*....*.

....*..........

...*...****....

...............

..**.*..*..*...

...*...**.*....

*..*...*.......

...............

.....*..*......

.........*.....


...............
```

the optimally placed eight is:

```plain
..88888888888..

..8.........8..

..8*******..8..

.*8...*.....8.*

.*8.....*...8*.

..8.*.......8..

..8*...****.8..

.88888888888888

.8**.*..*..*..8

.8.*...**.*...8

*8.*...*......8

.8............8

.8...*..*.....8

.8.......*....8

.88888888888888
```

The top rectangle has area $6 \times 9=54$, and the bottom rectangle has area $12 \times 6=72$. Thus, its aesthetic score is $54 \times 72=3888$.

## 输入格式

* Line $1$: A single integer $n$, indicating the side length of the marble.
* Lines $2..n+1$: Each line describes a row of the marble, and contains $n$ characters which are each either   `*`  (an imperfection) or  `.`  (a flawless section).
  
## 输出格式
  
  Line $1$: The highest aesthetic score of any figure eight which doesn't use any imperfect squares of the marble. If nofigure eight is attainable, then output `-1`.



```input1
15
...............

...............

...*******.....

.*....*.......*

.*......*....*.

....*..........

...*...****....

...............

..**.*..*..*...

...*...**.*....

*..*...*.......

...............

.....*..*......

.........*.....

...............
```



```output1
3888
```

## 数据规模与约定

对于 $100\%$ 的数据，$1 \le n \le 300$。

## 题目来源

Gold

