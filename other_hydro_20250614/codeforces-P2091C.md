## Description

<div><p>At the IT Campus "NEIMARK", there are several top-secret rooms where problems for major programming competitions are developed. To enter one of these rooms, you must unlock a circular lock by selecting the correct code. This code is updated every day.</p><p>Today's code is a permutation$^{\text{∗}}$ of the numbers from $1$ to $n$, with the property that in every cyclic shift$^{\text{†}}$ of it, there is exactly one fixed point. That is, in every cyclic shift, there exists exactly one element whose value is equal to its position in the permutation.</p><p>Output any valid permutation that satisfies this condition. Keep in mind that a valid permutation might not exist, then output $-1$.</p><div class="statement-footnote"><p>$^{\text{∗}}$A permutation is defined as a sequence of length $n$ consisting of integers from $1$ to $n$, where each number appears exactly once. For example, (2 1 3), (1), (4 3 1 2) are permutations; (1 2 2), (3), (1 3 2 5) are not.</p><p>$^{\text{†}}$A cyclic shift of an array is obtained by moving the last element to the beginning of the array. A permutation of length $n$ has exactly $n$ cyclic shifts.</p></div></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \leq t \leq 500$). The description of the test cases follows.</p><p>A single line of each test case contains a single integer $n$ ($1 \leq n \leq 2 \cdot 10^5$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output the desired permutation. If multiple solutions exist, output any one of them. If no suitable permutations exist, output $-1$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \leq t \leq 500$). The description of the test cases follows.</p><p>A single line of each test case contains a single integer $n$ ($1 \leq n \leq 2 \cdot 10^5$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output the desired permutation. If multiple solutions exist, output any one of them. If no suitable permutations exist, output $-1$.</p>





```input1|2,4
3
4
5
3
```




```output1
-1
4 1 3 5 2
1 3 2
```



## Note

<p>In the second example, there is a permutation such that in each cyclic shift there is a fixed point (highlighted in dark red):</p><center> <img class="tex-graphics" src="./37201/file/FIRlxcDp.png" style="max-width: 100.0%;max-height: 100.0%;" width="1329px"> </center><p><span class="tex-font-style-it">The first line contains the element numbers, and the second line contains all the shifts of the desired permutation.</span></p>
