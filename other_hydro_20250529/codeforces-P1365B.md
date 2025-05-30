## Description

<div><p>Ashish has $n$ elements arranged in a line. </p><p>These elements are represented by two integers $a_i$&nbsp;！ the value of the element and $b_i$&nbsp;！ the type of the element (there are only two possible types: $0$ and $1$). He wants to sort the elements in non-decreasing values of $a_i$.</p><p>He can perform the following operation any number of times: </p><ul><li> Select any two elements $i$ and $j$ such that $b_i \ne b_j$ and swap them. That is, he can only swap two elements of different types in one move. </li></ul><p>Tell him if he can sort the elements in non-decreasing values of $a_i$ after performing any number of operations.</p></div><div class="input-specification"><p>The first line contains one integer $t$ $(1 \le t \le 100)$&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains one integer $n$ $(1 \le n \le 500)$&nbsp;！ the size of the arrays.</p><p>The second line contains $n$ integers $a_i$ $(1 \le a_i \le 10^5)$ &nbsp;！ the value of the $i$-th element.</p><p>The third line containts $n$ integers $b_i$ $(b_i \in \{0, 1\})$ &nbsp;！ the type of the $i$-th element.</p></div><div class="output-specification"><p>For each test case, print "<span class="tex-font-style-tt">Yes</span>" or "<span class="tex-font-style-tt">No</span>" (without quotes) depending on whether it is possible to sort elements in non-decreasing order of their value.</p><p>You may print each letter in any case (upper or lower).</p></div>

## Input

<p>The first line contains one integer $t$ $(1 \le t \le 100)$&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains one integer $n$ $(1 \le n \le 500)$&nbsp;！ the size of the arrays.</p><p>The second line contains $n$ integers $a_i$ $(1 \le a_i \le 10^5)$ &nbsp;！ the value of the $i$-th element.</p><p>The third line containts $n$ integers $b_i$ $(b_i \in \{0, 1\})$ &nbsp;！ the type of the $i$-th element.</p>

## Output

<p>For each test case, print "<span class="tex-font-style-tt">Yes</span>" or "<span class="tex-font-style-tt">No</span>" (without quotes) depending on whether it is possible to sort elements in non-decreasing order of their value.</p><p>You may print each letter in any case (upper or lower).</p>

## Samples

```input1
5
4
10 20 20 30
0 1 0 1
3
3 1 2
0 1 1
4
2 2 4 8
1 1 1 1
3
5 15 4
0 0 0
4
20 10 100 50
1 0 0 1
```

```output1
Yes
Yes
Yes
No
Yes
```




## Note

<p>For the first case: The elements are already in sorted order.</p><p>For the second case: Ashish may first swap elements at positions $1$ and $2$, then swap elements at positions $2$ and $3$.</p><p>For the third case: The elements are already in sorted order.</p><p>For the fourth case: No swap operations may be performed as there is no pair of elements $i$ and $j$ such that $b_i \ne b_j$. The elements cannot be sorted.</p><p>For the fifth case: Ashish may swap elements at positions $3$ and $4$, then elements at positions $1$ and $2$.</p>
