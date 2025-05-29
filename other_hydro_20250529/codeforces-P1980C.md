## Description

<div><p>Sofia had an array of $n$ integers $a_1, a_2, \ldots, a_n$. One day she got bored with it, so she decided to <span class="tex-font-style-bf">sequentially</span> apply $m$ modification operations to it.</p><p>Each modification operation is described by a pair of numbers $\langle c_j, d_j \rangle$ and means that the element of the array with index $c_j$ should be assigned the value $d_j$, i.e., perform the assignment $a_{c_j} = d_j$. After applying <span class="tex-font-style-bf">all</span> modification operations <span class="tex-font-style-bf">sequentially</span>, Sofia discarded the resulting array.</p><p>Recently, you found an array of $n$ integers $b_1, b_2, \ldots, b_n$. You are interested in whether this array is Sofia's array. You know the values of the original array, as well as the values $d_1, d_2, \ldots, d_m$. The values $c_1, c_2, \ldots, c_m$ turned out to be lost.</p><p>Is there a sequence $c_1, c_2, \ldots, c_m$ such that the <span class="tex-font-style-bf">sequential</span> application of modification operations $\langle c_1, d_1, \rangle, \langle c_2, d_2, \rangle, \ldots, \langle c_m, d_m \rangle$ to the array $a_1, a_2, \ldots, a_n$ transforms it into the array $b_1, b_2, \ldots, b_n$?</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>Then follow the descriptions of the test cases.</p><p>The first line of each test case contains an integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;！ the size of the array.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;！ the elements of the original array.</p><p>The third line of each test case contains $n$ integers $b_1, b_2, \ldots, b_n$ ($1 \le b_i \le 10^9$)&nbsp;！ the elements of the found array.</p><p>The fourth line contains an integer $m$ ($1 \le m \le 2 \cdot 10^5$)&nbsp;！ the number of modification operations.</p><p>The fifth line contains $m$ integers $d_1, d_2, \ldots, d_m$ ($1 \le d_j \le 10^9$)&nbsp;！ the preserved value for each modification operation.</p><p>It is guaranteed that the sum of the values of $n$ for all test cases does not exceed $2 \cdot 10^5$, similarly the sum of the values of $m$ for all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>Output $t$ lines, each of which is the answer to the corresponding test case. As an answer, output "<span class="tex-font-style-tt">YES</span>" if there exists a suitable sequence $c_1, c_2, \ldots, c_m$, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can output the answer in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive answer).</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>Then follow the descriptions of the test cases.</p><p>The first line of each test case contains an integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;！ the size of the array.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;！ the elements of the original array.</p><p>The third line of each test case contains $n$ integers $b_1, b_2, \ldots, b_n$ ($1 \le b_i \le 10^9$)&nbsp;！ the elements of the found array.</p><p>The fourth line contains an integer $m$ ($1 \le m \le 2 \cdot 10^5$)&nbsp;！ the number of modification operations.</p><p>The fifth line contains $m$ integers $d_1, d_2, \ldots, d_m$ ($1 \le d_j \le 10^9$)&nbsp;！ the preserved value for each modification operation.</p><p>It is guaranteed that the sum of the values of $n$ for all test cases does not exceed $2 \cdot 10^5$, similarly the sum of the values of $m$ for all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>Output $t$ lines, each of which is the answer to the corresponding test case. As an answer, output "<span class="tex-font-style-tt">YES</span>" if there exists a suitable sequence $c_1, c_2, \ldots, c_m$, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can output the answer in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive answer).</p>





```input1|2,3,4,5,6,12,13,14,15,16,22,23,24,25,26,32,33,34,35,36
7
3
1 2 1
1 3 2
4
1 3 1 2
4
1 2 3 5
2 1 3 5
2
2 3
5
7 6 1 10 10
3 6 1 11 11
3
4 3 11
4
3 1 7 8
2 2 7 10
5
10 3 2 2 1
5
5 7 1 7 9
4 10 1 2 9
8
1 1 9 8 7 2 10 4
4
1000000000 203 203 203
203 1000000000 203 1000000000
2
203 1000000000
1
1
1
5
1 3 4 5 1
```




```output1
YES
NO
NO
NO
YES
NO
YES
```


