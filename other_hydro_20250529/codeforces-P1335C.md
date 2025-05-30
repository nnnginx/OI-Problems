## Description

<div><p>You have $n$ students under your control and you have to compose <span class="tex-font-style-bf">exactly two teams</span> consisting of some subset of your students. Each student had his own skill, the $i$-th student skill is denoted by an integer $a_i$ (different students can have the same skills).</p><p>So, about the teams. Firstly, these two teams should have the same size. Two more constraints:</p><ul> <li> The first team should consist of students with <span class="tex-font-style-bf">distinct</span> skills (i.e. all skills in the first team are unique). </li><li> The second team should consist of students with <span class="tex-font-style-bf">the same</span> skills (i.e. all skills in the second team are equal). </li></ul><p>Note that it is permissible that some student of the first team has the same skill as a student of the second team.</p><p>Consider some examples (skills are given):</p><ul> <li> $[1, 2, 3]$, $[4, 4]$ is not a good pair of teams because sizes should be the same; </li><li> $[1, 1, 2]$, $[3, 3, 3]$ is not a good pair of teams because the first team should not contain students with the same skills; </li><li> $[1, 2, 3]$, $[3, 4, 4]$ is not a good pair of teams because the second team should contain students with the same skills; </li><li> $[1, 2, 3]$, $[3, 3, 3]$ is a good pair of teams; </li><li> $[5]$, $[6]$ is a good pair of teams. </li></ul><p>Your task is to find the maximum possible size $x$ for which it is possible to compose a valid pair of teams, where each team size is $x$ (skills in the first team needed to be unique, skills in the second team should be the same between them). A student cannot be part of more than one team.</p><p>You have to answer $t$ independent test cases.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 10^4$) ！ the number of test cases. Then $t$ test cases follow.</p><p>The first line of the test case contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) ！ the number of students. The second line of the test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le n$), where $a_i$ is the skill of the $i$-th student. Different students can have the same skills.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$ ($\sum n \le 2 \cdot 10^5$).</p></div><div class="output-specification"><p>For each test case, print the answer ！ the maximum possible size $x$ for which it is possible to compose a valid pair of teams, where each team size is $x$.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 10^4$) ！ the number of test cases. Then $t$ test cases follow.</p><p>The first line of the test case contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) ！ the number of students. The second line of the test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le n$), where $a_i$ is the skill of the $i$-th student. Different students can have the same skills.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$ ($\sum n \le 2 \cdot 10^5$).</p>

## Output

<p>For each test case, print the answer ！ the maximum possible size $x$ for which it is possible to compose a valid pair of teams, where each team size is $x$.</p>

## Samples

```input1
4
7
4 2 4 1 4 3 4
5
2 1 5 4 3
1
1
4
1 1 1 3
```

```output1
3
1
0
2
```




## Note

<p>In the first test case of the example, it is possible to construct two teams of size $3$: the first team is $[1, 2, 4]$ and the second team is $[4, 4, 4]$. Note, that there are some other ways to construct two valid teams of size $3$.</p>
