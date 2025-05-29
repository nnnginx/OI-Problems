## Description

<div><p>You are given an integer array $a$ of size $n$.</p><p>You can perform the following operations any number of times (possibly, zero): </p><ul> <li> pay one coin and increase any element of the array by $1$ (you must have at least $1$ coin to perform this operation); </li><li> gain one coin and decrease any element of the array by $1$. </li></ul><p>Let's say that an array is <span class="tex-font-style-it">ideal</span> if both of the following conditions hold: </p><ul> <li> each element of the array is at least $2$; </li><li> for each pair of indices $i$ and $j$ ($1 \le i, j \le n$; $i \ne j$) the greatest common divisor (GCD) of $a_i$ and $a_j$ is equal to $1$. If the array has less than $2$ elements, this condition is automatically satisfied. </li></ul><p>Let's say that an array is <span class="tex-font-style-it">beautiful</span> if it can be transformed into an ideal array using the aforementioned operations, provided that you initially have no coins. If the array is already ideal, then it is also beautiful.</p><p>The given array is not necessarily beautiful or ideal. You can remove any elements from it (including removing the entire array or not removing anything at all). Your task is to calculate the minimum number of elements you have to remove (possibly, zero) from the array $a$ to make it <span class="tex-font-style-bf">beautiful</span>.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 4 \cdot 10^5$).</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($2 \le a_i \le 10^9$).</p><p>Additional constraint on the input: the sum of $n$ over all test cases doesn't exceed $4 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print a single integer&nbsp;！ the minimum number of elements you have to remove (possibly, zero) from the array $a$ to make it <span class="tex-font-style-bf">beautiful</span>.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 4 \cdot 10^5$).</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($2 \le a_i \le 10^9$).</p><p>Additional constraint on the input: the sum of $n$ over all test cases doesn't exceed $4 \cdot 10^5$.</p>

## Output

<p>For each test case, print a single integer&nbsp;！ the minimum number of elements you have to remove (possibly, zero) from the array $a$ to make it <span class="tex-font-style-bf">beautiful</span>.</p>





```input1|2,3,6,7,10,11
5
3
5 5 5
4
2 3 2 4
1
3
3
2 100 2
5
2 4 2 11 2
```




```output1
0
2
0
0
1
```



## Note

<p>In the first example, you don't need to delete any elements, because the array is already beautiful. It can be transformed into an ideal array as follows: $[5, 5, 5] \rightarrow [4, 5, 5] \rightarrow [4, 4, 5] \rightarrow [4, 3, 5]$ (you end up with $3$ coins).</p><p>In the second example, you need to remove $2$ elements so that the array becomes beautiful. If you leave the elements $[2, 3]$ and delete the other elements, then the given array is already ideal (and therefore, beautiful).</p><p>In the third example, you don't need to delete any elements because the array is already ideal (and thus, beautiful).</p><p>In the fourth example, the array is beautiful. It can be transformed into an ideal array as follows: $[2, 100, 2] \rightarrow [2, 99, 2] \rightarrow [2, 99, 3] \rightarrow [2, 98, 3] \rightarrow [2, 97, 3]$ (you end up with $2$ coins).</p>
