## Description

<div><p>Rumors of the excellence of Gabriella's wine tasting events have toured the world and made it to the headlines of prestigious wine magazines. Now, she has been asked to organize an event at the EUC 2025!</p><p>This time she selected $2n$ bottles of wine, of which exactly $n$ are of white wine, and exactly $n$ of red wine. She arranged them in a line as usual, in a predetermined order described by a string $s$ of length $2n$: for $1 \le i \le 2n$, the $i$-th bottle from the left is white wine if $s_i = \texttt{W}$ and red wine if $s_i = \texttt{R}$.</p><p>To spice things up for the attendees (which include EUC contestants), Gabriella came up with the following wine-themed problem:</p><p>Consider a way of dividing the $2n$ bottles into two disjoint subsets, each containing $n$ bottles. Then, for every $1 \le i \le n$, swap the $i$-th bottle in the first subset (from the left) and the $i$-th bottle of the second subset (also from the left). Is it possible to choose the subsets so that, after this operation is done exactly once, the white wines occupy the first $n$ positions?</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 500$) ！ the number of test cases. The descriptions of the $t$ test cases follow.</p><p>The first line of each test case contains an integer $n$ ($1 \le n \le 100$) ！ where $2n$ is the total number of bottles.</p><p>The second line of each test case contains a string $s$ of length $2n$, describing the bottle arrangement ！ the $i$-th character of $s$ ($1 \le i \le 2n$) is $\texttt{W}$ for a white wine and $\texttt{R}$ for a red wine.</p><p>It is guaranteed that $s$ contains exactly $n$ $\texttt{W}$'s and $n$ $\texttt{R}$'s.</p></div><div class="output-specification"><p>For each test case, print $\texttt{YES}$ if it is possible to divide the bottles as explained in the statement. Otherwise, print $\texttt{NO}$.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 500$) ！ the number of test cases. The descriptions of the $t$ test cases follow.</p><p>The first line of each test case contains an integer $n$ ($1 \le n \le 100$) ！ where $2n$ is the total number of bottles.</p><p>The second line of each test case contains a string $s$ of length $2n$, describing the bottle arrangement ！ the $i$-th character of $s$ ($1 \le i \le 2n$) is $\texttt{W}$ for a white wine and $\texttt{R}$ for a red wine.</p><p>It is guaranteed that $s$ contains exactly $n$ $\texttt{W}$'s and $n$ $\texttt{R}$'s.</p>

## Output

<p>For each test case, print $\texttt{YES}$ if it is possible to divide the bottles as explained in the statement. Otherwise, print $\texttt{NO}$.</p>





```input1|2,3,6,7
3
4
WRRWWWRR
1
WR
20
WWWWRRWRRRRRWRRWRWRRWRRWWWWWWWRWWRWWRRRR
```




```output1
YES
NO
YES
```



## Note

<p>In the <span class="tex-font-style-bf">first test case</span>, we can make one subset out of the bottles at positions $1$, $2$, $3$ and $7$ (which are, respectively: white, red, red, red) and the other subset out of the bottles at positions $4$, $5$, $6$, $8$ (which are, respectively: white, white, white, red). We will then swap pairs $(1, 4)$, $(2, 5)$, $(3, 6)$ and $(7, 8)$, after which the white wines will occupy the first $4$ positions, and the red wines the last $4$ positions.</p><p>In the <span class="tex-font-style-bf">second test case</span>, there is only one possible way to form the subsets: one with the first bottle, and one with the second bottle. After swapping, the resulting arrangement is $\texttt{RW}$, therefore there is no solution.</p>
