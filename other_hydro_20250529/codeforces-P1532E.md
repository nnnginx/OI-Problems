## Description

<div><p>Let's call an array <span class="tex-font-style-it">good</span> if there is an element in the array that equals to the sum of all other elements. For example, the array $a=[1, 3, 3, 7]$ is good because there is the element $a_4=7$ which equals to the sum $1 + 3 + 3$.</p><p>You are given an array $a$ consisting of $n$ integers. Your task is to print all indices $j$ of this array such that after removing the $j$-th element from the array it will be <span class="tex-font-style-it">good</span> (let's call such indices <span class="tex-font-style-it">nice</span>).</p><p>For example, if $a=[8, 3, 5, 2]$, the <span class="tex-font-style-it">nice</span> indices are $1$ and $4$: </p><ul> <li> if you remove $a_1$, the array will look like $[3, 5, 2]$ and it is <span class="tex-font-style-it">good</span>; </li><li> if you remove $a_4$, the array will look like $[8, 3, 5]$ and it is <span class="tex-font-style-it">good</span>. </li></ul><p>You have to consider all removals <span class="tex-font-style-bf">independently</span>, i. e. remove the element, check if the resulting array is <span class="tex-font-style-it">good</span>, and return the element into the array.</p></div><div class="input-specification"><p>The first line of the input contains one integer $n$ ($2 \le n \le 2 \cdot 10^5$) — the number of elements in the array $a$.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^6$) — elements of the array $a$.</p></div><div class="output-specification"><p>In the first line print one integer $k$ — the number of indices $j$ of the array $a$ such that after removing the $j$-th element from the array it will be <span class="tex-font-style-it">good</span> (i.e. print the number of the <span class="tex-font-style-it">nice</span> indices).</p><p>In the second line print $k$ distinct integers $j_1, j_2, \dots, j_k$ in <span class="tex-font-style-bf">any</span> order — <span class="tex-font-style-it">nice</span> indices of the array $a$.</p><p>If there are no such indices in the array $a$, just print $0$ in the first line and leave the second line empty or do not print it at all.</p></div>

## Input

<p>The first line of the input contains one integer $n$ ($2 \le n \le 2 \cdot 10^5$) — the number of elements in the array $a$.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^6$) — elements of the array $a$.</p>

## Output

<p>In the first line print one integer $k$ — the number of indices $j$ of the array $a$ such that after removing the $j$-th element from the array it will be <span class="tex-font-style-it">good</span> (i.e. print the number of the <span class="tex-font-style-it">nice</span> indices).</p><p>In the second line print $k$ distinct integers $j_1, j_2, \dots, j_k$ in <span class="tex-font-style-bf">any</span> order — <span class="tex-font-style-it">nice</span> indices of the array $a$.</p><p>If there are no such indices in the array $a$, just print $0$ in the first line and leave the second line empty or do not print it at all.</p>

## Samples

```input1
5
2 5 1 2 2
```

```output1
3
4 1 5
```






```input2
4
8 3 5 2
```

```output2
2
1 4
```






```input3
5
2 1 2 4 3
```

```output3
0
```




## Note

<p>In the first example you can remove any element with the value $2$ so the array will look like $[5, 1, 2, 2]$. The sum of this array is $10$ and there is an element equals to the sum of remaining elements ($5 = 1 + 2 + 2$).</p><p>In the second example you can remove $8$ so the array will look like $[3, 5, 2]$. The sum of this array is $10$ and there is an element equals to the sum of remaining elements ($5 = 3 + 2$). You can also remove $2$ so the array will look like $[8, 3, 5]$. The sum of this array is $16$ and there is an element equals to the sum of remaining elements ($8 = 3 + 5$).</p><p>In the third example you cannot make the given array <span class="tex-font-style-it">good</span> by removing exactly one element.</p>
