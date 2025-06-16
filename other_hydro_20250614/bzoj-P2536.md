## Description

One famous Russian architect plans to build a new monumental construction. It will be a huge clock that indicates the time from the beginning of the universe.

The face of this clock contains hands, moving at constant speeds. They are numbered from $1$ to $n$ from the fastest to the slowest one. The fastest hand makes one revolution per minute ($60$ seconds). Each next hand moves slower than previous, the $(i + 1)$-th hand makes one revolution when the $i$-th hand makes $d_i$ revolutions.

The setting mechanism of this clock is very simple. You can take a hand by the handle, located on its end, and move it in any direction. When you move the hand, slower hands are moving in proportion to their usual speeds, and faster hands are not moving. Remember that hands are huge, so setting this clock is a hard job.

Consider an example with three hands: a second hand, a minute hand, and an hour hand. Their lengths are $5,\ 15$ and $10$ meters respectively. You want to set the clock from $2:30$ to $6:00$. The easiest way to do it is to rotate the minute hand $180^\circ$ clockwise, and then move the hour hand $90^\circ$ clockwise.

The total distance you moved the handles of the hands is approximately $62.83$ meters.

![](./2086/file/pic1.png)

Your task is to write a program that finds the way to set the clock that minimizes the total distance you have to move the handles.

## Input

The first line of the input file contains one integer $n$ - the number of hands ($0 < n \leq 50$). The second line contains $n − 1$ integer numbers $d_1,\ d_2,\ \cdots,\ d_{n−1}$ ($2 \leq d_i \leq 10^6$). The third line contains $n$ integer numbers $l_1,\ l_2,\ \cdots,\ l_n$ ($1 \leq l_i \leq 10^6$) - lengths of clock hands. Next two lines contain two non-negative integer numbers (one number per line): time indicated by the clock and the actual time that should be set. Both times are measured in seconds from the beginning of the universe and are less than $263$.

## Output

Print the minimal possible total distance you have to move the handles. The answer must be precise toat least $4$ digits after decimal point.

```input1
3
60 12
5 15 10
52200
453600
```

```output1
62.831853072
```