## Description

<div><p>Sonya decided that having her own hotel business is the best way of earning money because she can profit and rest wherever she wants.</p><p>The country where Sonya lives is an endless line. There is a city in each integer coordinate on this line. She has $n$ hotels, where the $i$-th hotel is located in the city with coordinate $x_i$. Sonya is a smart girl, so she does not open two or more hotels in the same city.</p><p>Sonya understands that her business needs to be expanded by opening new hotels, so she decides to build one more. She wants to make the minimum distance from this hotel to all others to be equal to $d$. The girl understands that there are many possible locations to construct such a hotel. Thus she wants to know the number of possible coordinates of the cities where she can build a new hotel. </p><p>Because Sonya is lounging in a jacuzzi in one of her hotels, she is asking you to find the number of cities where she can build a new hotel so that the minimum distance from the original $n$ hotels to the new one is equal to $d$.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $d$ ($1\leq n\leq 100$, $1\leq d\leq 10^9$)&nbsp;�� the number of Sonya's hotels and the needed minimum distance from a new hotel to all others.</p><p>The second line contains $n$ different integers in strictly increasing order $x_1, x_2, \ldots, x_n$ ($-10^9\leq x_i\leq 10^9$)&nbsp;�� coordinates of Sonya's hotels.</p></div><div class="output-specification"><p>Print the number of cities where Sonya can build a new hotel so that the minimum distance from this hotel to all others is equal to $d$.</p></div>

## Input

<p>The first line contains two integers $n$ and $d$ ($1\leq n\leq 100$, $1\leq d\leq 10^9$)&nbsp;�� the number of Sonya's hotels and the needed minimum distance from a new hotel to all others.</p><p>The second line contains $n$ different integers in strictly increasing order $x_1, x_2, \ldots, x_n$ ($-10^9\leq x_i\leq 10^9$)&nbsp;�� coordinates of Sonya's hotels.</p>

## Output

<p>Print the number of cities where Sonya can build a new hotel so that the minimum distance from this hotel to all others is equal to $d$.</p>

## Samples

```input1
4 3
-3 2 9 16

```

```output1
6

```






```input2
5 2
4 8 11 18 19

```

```output2
5

```




## Note

<p>In the first example, there are $6$ possible cities where Sonya can build a hotel. These cities have coordinates $-6$, $5$, $6$, $12$, $13$, and $19$.</p><p>In the second example, there are $5$ possible cities where Sonya can build a hotel. These cities have coordinates $2$, $6$, $13$, $16$, and $21$.</p>
