## Description

<div><p>Tim is doing a test consisting of $4n$ questions; each question has $4$ options: '<span class="tex-font-style-tt">A</span>', '<span class="tex-font-style-tt">B</span>', '<span class="tex-font-style-tt">C</span>', and '<span class="tex-font-style-tt">D</span>'. For each option, there are exactly $n$ correct answers corresponding to that option ！ meaning there are $n$ questions with the answer '<span class="tex-font-style-tt">A</span>', $n$ questions with the answer '<span class="tex-font-style-tt">B</span>', $n$ questions with the answer '<span class="tex-font-style-tt">C</span>', and $n$ questions with the answer '<span class="tex-font-style-tt">D</span>'.</p><p>For each question, Tim wrote his answer on the answer sheet. If he could not figure out the answer, he would leave a question mark '<span class="tex-font-style-tt">?</span>' for that question.</p><p>You are given his answer sheet of $4n$ characters. What is the maximum number of correct answers Tim can get?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains an integer $n$ ($1 \le n \le 100$).</p><p>The second line of each test case contains a string $s$ of $4n$ characters ($s_i \in \{\texttt{A}, \texttt{B}, \texttt{C}, \texttt{D}, \texttt{?}\}$)&nbsp;！ Tim's answers for the questions.</p></div><div class="output-specification"><p>For each test case, print a single integer&nbsp;！ the maximum score that Tim can achieve.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains an integer $n$ ($1 \le n \le 100$).</p><p>The second line of each test case contains a string $s$ of $4n$ characters ($s_i \in \{\texttt{A}, \texttt{B}, \texttt{C}, \texttt{D}, \texttt{?}\}$)&nbsp;！ Tim's answers for the questions.</p>

## Output

<p>For each test case, print a single integer&nbsp;！ the maximum score that Tim can achieve.</p>





```input1|2,3,6,7,10,11
6
1
ABCD
2
AAAAAAAA
2
AAAABBBB
2
????????
3
ABCABCABCABC
5
ACADC??ACAC?DCAABC?C
```




```output1
4
2
4
0
9
13
```



## Note

<p>In the first test case, there is exactly one question with each answer '<span class="tex-font-style-tt">A</span>', '<span class="tex-font-style-tt">B</span>', '<span class="tex-font-style-tt">C</span>', and '<span class="tex-font-style-tt">D</span>'; so it's possible that Tim gets all his answers correct.</p><p>In the second test case, there are only two correct answers '<span class="tex-font-style-tt">A</span>' which makes him get exactly $2$ points in any case.</p><p>In the third test case, Tim can get at most $2$ correct answers with option '<span class="tex-font-style-tt">A</span>' and $2$ correct answers with option '<span class="tex-font-style-tt">B</span>'. For example, he would get $4$ points if the answers were '<span class="tex-font-style-tt">AACCBBDD</span>'.</p><p>In the fourth test case, he refuses to answer any question at all, which makes him get $0$ points.</p>
