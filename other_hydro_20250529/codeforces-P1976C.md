## Description

<div><p>Monocarp is opening his own IT company. He wants to hire $n$ programmers and $m$ testers. </p><p>There are $n+m+1$ candidates, numbered from $1$ to $n+m+1$ in chronological order of their arriving time. The $i$-th candidate has programming skill $a_i$ and testing skill $b_i$ (a person's programming skill is different from their testing skill). The skill of the team is the sum of the programming skills of all candidates hired as programmers, and the sum of the testing skills of all candidates hired as testers.</p><p>When a candidate arrives to interview, Monocarp tries to assign them to the most suitable position for them (if their programming skill is higher, then he hires them as a programmer, otherwise as a tester). If all slots for that position are filled, Monocarp assigns them to the other position.</p><p>Your task is, for each candidate, calculate the skill of the team if everyone except them comes to interview. Note that it means that exactly $n+m$ candidates will arrive, so all $n+m$ positions in the company will be filled.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>Each test case consists of three lines:</p><ul> <li> the first line contains two integers $n$ and $m$ ($0 \le n, m \le 2 \cdot 10^5$; $2 \le n + m + 1 \le 2 \cdot 10^5$)&nbsp;！ the number of programmers and the number of testers Monocarp wants to hire, respectively; </li><li> the second line contains $n + m + 1$ integers $a_1, a_2, \dots, a_{n+m+1}$ ($1 \le a_i \le 10^9$), where $a_i$ is the programming skill of the $i$-th candidate; </li><li> the third line contains $n + m + 1$ integers $b_1, b_2, \dots, b_{n+m+1}$ ($1 \le b_i \le 10^9$; $b_i \ne a_i$), where $b_i$ is the testing skill of the $i$-th candidate. </li></ul><p>Additional constraint on the input: the sum of $(n + m + 1)$ over all test cases doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print $n + m + 1$ integers, where the $i$-th integer should be equal to the skill of the team if everyone except the $i$-th candidate comes to interview.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>Each test case consists of three lines:</p><ul> <li> the first line contains two integers $n$ and $m$ ($0 \le n, m \le 2 \cdot 10^5$; $2 \le n + m + 1 \le 2 \cdot 10^5$)&nbsp;！ the number of programmers and the number of testers Monocarp wants to hire, respectively; </li><li> the second line contains $n + m + 1$ integers $a_1, a_2, \dots, a_{n+m+1}$ ($1 \le a_i \le 10^9$), where $a_i$ is the programming skill of the $i$-th candidate; </li><li> the third line contains $n + m + 1$ integers $b_1, b_2, \dots, b_{n+m+1}$ ($1 \le b_i \le 10^9$; $b_i \ne a_i$), where $b_i$ is the testing skill of the $i$-th candidate. </li></ul><p>Additional constraint on the input: the sum of $(n + m + 1)$ over all test cases doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print $n + m + 1$ integers, where the $i$-th integer should be equal to the skill of the team if everyone except the $i$-th candidate comes to interview.</p>





```input1|2,3,4,8,9,10
4
1 0
2 1
1 2
0 2
4 5 5
5 4 1
1 2
2 1 5 4
5 2 3 1
3 1
4 3 3 4 1
5 5 4 5 2
```




```output1
1 2 
5 6 9 
8 11 11 12 
13 13 13 12 15
```



## Note

<p>Let's consider the third test case of the example:</p><ul> <li> if the $1$-st candidate does not arrive, the $2$-nd candidate gets hired as a tester, the $3$-rd candidate gets hired as a programmer, the $4$-th candidate gets hired as a tester. The total skill of the team will be $2 + 5 + 1 = 8$; </li><li> if the $2$-nd candidate does not arrive, the $1$-st candidate gets hired as a tester, the $3$-rd candidate gets hired as a programmer, the $4$-th candidate gets hired as a tester. The total skill of the team will be $5 + 5 + 1 = 11$; </li><li> if the $3$-rd candidate does not arrive, the $1$-st candidate gets hired as a tester, the $2$-nd candidate gets hired as a tester, the $4$-th candidate gets hired as a programmer. The total skill of the team will be $5 + 2 + 4 = 11$; </li><li> if the $4$-th candidate does not arrive, the $1$-st candidate gets hired as a tester, the $2$-nd candidate gets hired as a tester, the $3$-rd candidate gets hired as a programmer. The total skill of the team will be $5 + 2 + 5 = 12$. </li></ul>
