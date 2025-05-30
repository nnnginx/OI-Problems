## Description

<div><p>You've been in love with Coronavirus-chan for a long time, but you didn't know where she lived until now. And just now you found out that she lives in a faraway place called Naha. </p><p>You immediately decided to take a vacation and visit Coronavirus-chan. Your vacation lasts exactly $x$ days and that's the exact number of days you will spend visiting your friend. You will spend exactly $x$ consecutive (successive) days visiting Coronavirus-chan.</p><p>They use a very unusual calendar in Naha: there are $n$ months in a year, $i$-th month lasts exactly $d_i$ days. Days in the $i$-th month are numbered from $1$ to $d_i$. There are no leap years in Naha.</p><p>The mood of Coronavirus-chan (and, accordingly, her desire to hug you) depends on the number of the day in a month. In particular, you get $j$ hugs if you visit Coronavirus-chan on the $j$-th day of the month.</p><p>You know about this feature of your friend and want to plan your trip to get as many hugs as possible (and then maybe you can win the heart of Coronavirus-chan). </p><p>Please note that your trip should <span class="tex-font-style-bf">not necessarily</span> begin and end in the same year.</p></div><div class="input-specification"><p>The first line of input contains two integers $n$ and $x$ ($1 \le n \le 2 \cdot 10^5$) �� the number of months in the year and the number of days you can spend with your friend.</p><p>The second line contains $n$ integers $d_1, d_2, \ldots, d_n$, $d_i$ is the number of days in the $i$-th month ($1 \le d_i \le 10^6$).</p><p>It is guaranteed that $1 \le x \le d_1 + d_2 + \ldots + d_n$.</p></div><div class="output-specification"><p>Print one integer �� the maximum number of hugs that you can get from Coronavirus-chan during the best vacation in your life.</p></div>

## Input

<p>The first line of input contains two integers $n$ and $x$ ($1 \le n \le 2 \cdot 10^5$) �� the number of months in the year and the number of days you can spend with your friend.</p><p>The second line contains $n$ integers $d_1, d_2, \ldots, d_n$, $d_i$ is the number of days in the $i$-th month ($1 \le d_i \le 10^6$).</p><p>It is guaranteed that $1 \le x \le d_1 + d_2 + \ldots + d_n$.</p>

## Output

<p>Print one integer �� the maximum number of hugs that you can get from Coronavirus-chan during the best vacation in your life.</p>

## Samples

```input1
3 2
1 3 1
```

```output1
5
```






```input2
3 6
3 3 3
```

```output2
12
```






```input3
5 6
4 2 3 1 3
```

```output3
15
```




## Note

<p>In the first test case, the numbers of the days in a year are (indices of days in a corresponding month) $\{1,1,2,3,1\}$. Coronavirus-chan will hug you the most if you come on the third day of the year: $2+3=5$ hugs.</p><p>In the second test case, the numbers of the days are $\{1,2,3,1,2,3,1,2,3\}$. You will get the most hugs if you arrive on the third day of the year: $3+1+2+3+1+2=12$ hugs.</p><p>In the third test case, the numbers of the days are $\{1,2,3,4,1,2, 1,2,3, 1, 1,2,3\}$. You will get the most hugs if you come on the twelfth day of the year: your friend will hug you $2+3+1+2+3+4=15$ times. </p>
