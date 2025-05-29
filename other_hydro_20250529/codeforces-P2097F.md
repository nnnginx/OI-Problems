## Description

<div><p>As is known, the airline "Trouble" often loses luggage, and concerned journalists decided to calculate the maximum number of luggage pieces that may not return to travelers.</p><p>The airline "Trouble" operates flights between $n$ airports, numbered from $1$ to $n$. The journalists' experiment will last for $m$ days. It is known that at midnight before the first day of the experiment, there were $s_j$ lost pieces of luggage in the $j$-th airport. On the $i$-th day, the following occurs:</p><ul> <li> <span class="tex-font-style-bf">In the morning</span>, $2n$ flights take off simultaneously, including $n$ flights of the <span class="tex-font-style-it">first type</span> and $n$ flights of the <span class="tex-font-style-it">second type</span>. <ul> <li> The $j$-th flight of the first type flies from airport $j$ to airport $(((j-2) \bmod n )+ 1)$ (the previous airport, with the first airport being the last), and it can carry no more than $a_{i,j}$ lost pieces of luggage. </li><li> The $j$-th flight of the second type flies from airport $j$ to airport $((j \bmod n) + 1)$ (the next airport, with the last airport being the first), and it can carry no more than $c_{i,j}$ lost pieces of luggage. </li></ul> </li><li> <span class="tex-font-style-bf">In the afternoon</span>, a check of lost luggage is conducted at the airports. If after the flights have departed on that day, there are $x$ pieces of luggage remaining in the $j$-th airport and $x \ge b_{i, j}$, then at least $x - b_{i, j}$ pieces of luggage are found, and they <span class="tex-font-style-bf">cease to be lost</span>. </li><li> <span class="tex-font-style-bf">In the evening</span>, all $2n$ flights conclude, and the lost luggage transported that day arrives at the corresponding airports. </li></ul><p>For each $k$ from $1$ to $m$, the journalists want to know the maximum number of lost pieces of luggage that may be <span class="tex-font-style-bf">unfound</span> during the checks over the first $k$ days. Note that for each $k$, these values are calculated independently.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). The description of the test cases follows. </p><p>The first line of each test case contains two integers $n$ and $m$ ($3 \le n \le 12$, $1 \le m \le 2000$)&nbsp;！ the number of airports and the number of days of the experiment.</p><p>The second line of each test case contains $n$ integers $s_1, s_2, \ldots, s_n$ ($0 \le s_i \le 10^8$)&nbsp;！ the initial number of lost pieces of luggage in each airport.</p><p>Next, the descriptions for each of the $m$ days follow in order.</p><p>The first line of the description of the $i$-th day contains $n$ integers $a_{i,1}, a_{i,2}, \ldots, a_{i,n}$ ($0 \le a_{i, j} \le 10^8$)&nbsp;！ the maximum number of lost pieces of luggage that can be transported to the previous airport for each airport.</p><p>The second line of the description of the $i$-th day contains $n$ integers $b_{i,1}, \ldots, b_{i,n}$ ($0 \le b_{i, j} \le 10^8$)&nbsp;！ the minimum number of lost pieces of luggage that will be found on the $i$-th day in each airport.</p><p>The third line of the description of the $i$-th day contains $n$ integers $c_{i,1}, \ldots, c_{i,n}$ ($0 \le c_{i, j} \le 10^8$)&nbsp;！ the maximum number of lost pieces of luggage that can be transported to the next airport for each airport.</p><p>It is guaranteed that the sum of $m$ over all test cases does not exceed $2000$.</p></div><div class="output-specification"><p>For each test case, output $m$ integers&nbsp;！ the maximum number of unfound pieces of luggage for each number of days from $1$ to $m$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). The description of the test cases follows. </p><p>The first line of each test case contains two integers $n$ and $m$ ($3 \le n \le 12$, $1 \le m \le 2000$)&nbsp;！ the number of airports and the number of days of the experiment.</p><p>The second line of each test case contains $n$ integers $s_1, s_2, \ldots, s_n$ ($0 \le s_i \le 10^8$)&nbsp;！ the initial number of lost pieces of luggage in each airport.</p><p>Next, the descriptions for each of the $m$ days follow in order.</p><p>The first line of the description of the $i$-th day contains $n$ integers $a_{i,1}, a_{i,2}, \ldots, a_{i,n}$ ($0 \le a_{i, j} \le 10^8$)&nbsp;！ the maximum number of lost pieces of luggage that can be transported to the previous airport for each airport.</p><p>The second line of the description of the $i$-th day contains $n$ integers $b_{i,1}, \ldots, b_{i,n}$ ($0 \le b_{i, j} \le 10^8$)&nbsp;！ the minimum number of lost pieces of luggage that will be found on the $i$-th day in each airport.</p><p>The third line of the description of the $i$-th day contains $n$ integers $c_{i,1}, \ldots, c_{i,n}$ ($0 \le c_{i, j} \le 10^8$)&nbsp;！ the maximum number of lost pieces of luggage that can be transported to the next airport for each airport.</p><p>It is guaranteed that the sum of $m$ over all test cases does not exceed $2000$.</p>

## Output

<p>For each test case, output $m$ integers&nbsp;！ the maximum number of unfound pieces of luggage for each number of days from $1$ to $m$.</p>





```input1|2,3,4,5,6,7,8,9,10,11,12
2
5 3
1 1 1 1 1
0 0 1 0 0
0 1 0 0 1
1 0 0 1 0
0 1 0 0 0
9 0 9 9 9
0 1 0 0 0
0 0 0 0 0
9 0 9 0 0
0 0 0 0 0
3 1
0 100000000 5
0 100000000 5
0 100000000 5
0 100000000 5
```




```output1
5
4
2
100000005
```



## Note

<p>In the first test case: </p><ul> <li> On the first day, all $5$ pieces of luggage may not be found, as the lost luggage can be sent on flights from each airport.</li><li> In the morning of the second day, there may be no more than $3$ pieces of luggage in the $2$-nd airport, no more than $2$ pieces in the $5$-th airport, and no luggage in the other airports. All luggage from the $5$-th airport may remain there. In the $2$-nd airport, no more than $2$ pieces of luggage can be sent on flights to neighboring airports. Thus, at least $1$ piece of luggage will be found.</li><li> By the end of the third day, lost luggage may only be in the $1$-st and $2$-nd airports. There can be no more than one piece in each, meaning that at most $2$ pieces of luggage will remain unfound in total. </li></ul><center>  <img class="tex-graphics" src="./37152/file/JOoQs7yp.png" style="max-width: 100.0%;max-height: 100.0%;" width="450px">   <span class="tex-font-size-small">The found luggage is marked in green.</span> </center><p>In the second test case, all pieces of luggage may remain in their original airports, and the inspection won't find any lost suitcases. Therefore, the answer is $10^9 + 5$.</p>
