## Description

<div><p>FizzBuzz is one of the most well-known problems from coding interviews. In this problem, we will consider a remixed version of FizzBuzz:</p><p><span class="tex-font-style-it">Given an integer $n$, process all integers from $0$ to $n$. For every integer such that its remainders modulo $3$ and modulo $5$ are the same (so, for every integer $i$ such that $i \bmod 3 = i \bmod 5$), print</span> <span class="tex-font-style-tt">FizzBuzz</span>.</p><p>However, you don't have to solve it. Instead, given the integer $n$, you have to report how many times the correct solution to that problem will print <span class="tex-font-style-tt">FizzBuzz</span>.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10^4$) ！ the number of test cases.</p><p>Each test case contains one line consisting of one integer $n$ ($0 \le n \le 10^9$).</p></div><div class="output-specification"><p>For each test case, print one integer ！ the number of times the correct solution will print <span class="tex-font-style-tt">FizzBuzz</span> with the given value of $n$.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10^4$) ！ the number of test cases.</p><p>Each test case contains one line consisting of one integer $n$ ($0 \le n \le 10^9$).</p>

## Output

<p>For each test case, print one integer ！ the number of times the correct solution will print <span class="tex-font-style-tt">FizzBuzz</span> with the given value of $n$.</p>





```input1|2,4,6,8
7
0
5
15
42
1337
17101997
998244353
```




```output1
1
3
4
9
270
3420402
199648872
```



## Note

<p>In the first test case, the solution will print <span class="tex-font-style-tt">FizzBuzz</span> for the integer $0$.</p><p>In the second test case, the solution will print <span class="tex-font-style-tt">FizzBuzz</span> for the integers $0, 1, 2$.</p><p>In the third test case, the solution will print <span class="tex-font-style-tt">FizzBuzz</span> for the integers $0, 1, 2, 15$.</p>
