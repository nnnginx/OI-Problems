## Description

<div><p>You have been asked to organize a very important art conference. The first step is to choose the dates.</p><p>The conference must last for a certain number of consecutive days. Each day, one lecturer must perform, and the same lecturer cannot perform more than once.</p><p>You asked $n$ potential lecturers if they could participate in the conference. Lecturer $i$ indicated that they could perform on any day from $l_i$ to $r_i$ inclusive.</p><p>A certain segment of days can be chosen as the conference dates if there is a way to assign an available lecturer to each day of the segment, assigning each lecturer to no more than one day.</p><p>For each $k$ from $1$ to $n$, find how many ways there are to choose a segment of $k$ consecutive days as the conference dates.</p></div><div class="input-specification"><p>The first line of input contains one integer $n$&nbsp;�� the number of potential lecturers ($1 \le n \le 2 \cdot 10^5$).</p><p>Each of the next $n$ lines contains two integers $l_i$ and $r_i$&nbsp;�� the segment of available days for the $i$th lecturer ($1 \le l_i \le r_i \le 2 \cdot 10^5$).</p></div><div class="output-specification"><p>Print $n$ integers, where the $k$th number denotes the number of ways to select a segment of $k$ consecutive days as conference dates.</p></div>

## Input

<p>The first line of input contains one integer $n$&nbsp;�� the number of potential lecturers ($1 \le n \le 2 \cdot 10^5$).</p><p>Each of the next $n$ lines contains two integers $l_i$ and $r_i$&nbsp;�� the segment of available days for the $i$th lecturer ($1 \le l_i \le r_i \le 2 \cdot 10^5$).</p>

## Output

<p>Print $n$ integers, where the $k$th number denotes the number of ways to select a segment of $k$ consecutive days as conference dates.</p>





```input1|
3
1 2
3 4
5 6
```




```input2|
5
1 3
1 3
1 3
1 3
1 3
```




```output1
6
2
0
```




```output2
3
2
1
0
0
```



## Note

<p>In the first testcase, a one-day conference can be organized on any of the days from $1$ to $6$. A two-day conference can be organized from day $2$ to day $3$, as well as from day $4$ to day $5$.</p><p>In the second testcase, five lecturers can perform only from day $1$ to day $3$, so it will not be possible to organize a conference longer than three days.</p>
