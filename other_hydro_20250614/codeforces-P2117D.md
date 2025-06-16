## Description

<div><p>Yousef wants to explode an array $a_1, a_2, \dots, a_n$. An array gets exploded when all of its elements become equal to zero.</p><p>In one operation, Yousef can do <span class="tex-font-style-bf">exactly</span> one of the following: </p><ol> <li> For every index $i$ in $a$, decrease $a_i$ by $i$. </li><li> For every index $i$ in $a$, decrease $a_i$ by $n - i + 1$. </li></ol><p>Your task is to help Yousef determine if it is possible to explode the array using any number of operations.</p></div><div class="input-specification"><p>The first line of the input contains an integer $t$ ($1 \le t \le 10^4$) ！ the number of test cases.</p><p>The first line of each test case contains an integer $n$ ($2 \le n \le 2 \cdot 10^5$) ！ the size of the array.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$) ！ the elements of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print "<span class="tex-font-style-tt">YES</span>" if Yousef can explode the array, otherwise output "<span class="tex-font-style-tt">NO</span>".</p><p>You can output the answer in any case (upper or lower). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as positive responses.</p></div>

## Input

<p>The first line of the input contains an integer $t$ ($1 \le t \le 10^4$) ！ the number of test cases.</p><p>The first line of each test case contains an integer $n$ ($2 \le n \le 2 \cdot 10^5$) ！ the size of the array.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$) ！ the elements of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print "<span class="tex-font-style-tt">YES</span>" if Yousef can explode the array, otherwise output "<span class="tex-font-style-tt">NO</span>".</p><p>You can output the answer in any case (upper or lower). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as positive responses.</p>





```input1|2,3,6,7,10,11
6
4
3 6 6 3
5
21 18 15 12 9
10
2 6 10 2 5 5 1 2 4 10
7
10 2 16 12 8 20 4
2
52 101
2
10 2
```




```output1
NO
YES
NO
NO
YES
NO
```



## Note

<p>In the second test case, we can do the following: </p><ul> <li> Perform $1$ operation of the first type. The array becomes $[20, 16, 12, 8, 4]$. </li><li> Perform $4$ operations of the second type. The array becomes $[0, 0, 0, 0, 0]$. </li></ul><p>In the first, third, fourth, and sixth test cases, it can be proven that it is impossible to make all elements equal to zero using any number of operations.</p>
