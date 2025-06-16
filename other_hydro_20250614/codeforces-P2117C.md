## Description

<div><p>Yousef has an array $a$ of size $n$. He wants to partition the array into one or more contiguous segments such that each element $a_i$ belongs to exactly one segment.</p><p>A partition is called <span class="tex-font-style-it">cool</span> if, for every segment $b_j$, all elements in $b_j$ also appear in $b_{j + 1}$ (if it exists). That is, every element in a segment must also be present in the segment following it.</p><p>For example, if $a = [1, 2, 2, 3, 1, 5]$, a <span class="tex-font-style-it">cool</span> partition Yousef can make is $b_1 = [1, 2]$, $b_2 = [2, 3, 1, 5]$. This is a <span class="tex-font-style-it">cool</span> partition because every element in $b_1$ (which are $1$ and $2$) also appears in $b_2$. In contrast, $b_1 = [1, 2, 2]$, $b_2 = [3, 1, 5]$ is not a <span class="tex-font-style-it">cool</span> partition, since $2$ appears in $b_1$ but not in $b_2$.</p><p>Note that after partitioning the array, you do <span class="tex-font-style-bf">not</span> change the order of the segments. Also, note that if an element appears several times in some segment $b_j$, it only needs to appear at least once in $b_{j + 1}$.</p><p>Your task is to help Yousef by finding the maximum number of segments that make a <span class="tex-font-style-it">cool</span> partition.</p></div><div class="input-specification"><p>The first line of the input contains integer $t$ ($1 \le t \le 10^4$) ！ the number of test cases.</p><p>The first line of each test case contains an integer $n$ ($1 \le n \le 2 \cdot 10^5$) ！ the size of the array.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le n$) ！ the elements of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print one integer ！ the maximum number of segments that make a <span class="tex-font-style-it">cool</span> partition.</p></div>

## Input

<p>The first line of the input contains integer $t$ ($1 \le t \le 10^4$) ！ the number of test cases.</p><p>The first line of each test case contains an integer $n$ ($1 \le n \le 2 \cdot 10^5$) ！ the size of the array.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le n$) ！ the elements of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print one integer ！ the maximum number of segments that make a <span class="tex-font-style-it">cool</span> partition.</p>





```input1|2,3,6,7,10,11,14,15
8
6
1 2 2 3 1 5
8
1 2 1 3 2 1 3 2
5
5 4 3 2 1
10
5 8 7 5 8 5 7 8 10 9
3
1 2 2
9
3 3 1 4 3 2 4 1 2
6
4 5 4 5 6 4
8
1 2 1 2 1 2 1 2
```




```output1
2
3
1
3
1
3
3
4
```



## Note

<p>The first test case is explained in the statement. We can partition it into $b_1 = [1, 2]$, $b_2 = [2, 3, 1, 5]$. It can be shown there is no other partition with more segments.</p><p>In the second test case, we can partition the array into $b_1 = [1, 2]$, $b_2 = [1, 3, 2]$, $b_3 = [1, 3, 2]$. The maximum number of segments is $3$.</p><p>In the third test case, the only partition we can make is $b_1 = [5, 4, 3, 2, 1]$. Any other partition will not satisfy the condition. Therefore, the answer is $1$.</p>
