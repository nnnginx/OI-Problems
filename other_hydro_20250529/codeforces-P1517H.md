## Description

<div><p>After hearing the story of Dr. Zhang, Wowo decides to plan his own flight around the world. </p><p>He already chose $n$ checkpoints in the world map. Due to the landform and the clouds, he cannot fly too high or too low. Formally, let $b_i$ be the height of Wowo's aircraft at checkpoint $i$, $x_i^-\le b_i\le x_i^+$ should be satisfied for all integers $i$ between $1$ and $n$, where $x_i^-$ and $x_i^+$ are given integers.</p><p>The angle of Wowo's aircraft is also limited. For example, it cannot make a $90$-degree climb. Formally, $y_i^-\le b_i-b_{i-1}\le y_i^+$ should be satisfied for all integers $i$ between $2$ and $n$, where $y_i^-$ and $y_i^+$ are given integers.</p><p>The final limitation is the speed of angling up or angling down. An aircraft should change its angle slowly for safety concerns. Formally, $z_i^- \le (b_i - b_{i-1}) - (b_{i-1} - b_{i-2}) \le z_i^+$ should be satisfied for all integers $i$ between $3$ and $n$, where $z_i^-$ and $z_i^+$ are given integers.</p><p>Taking all these into consideration, Wowo finds that the heights at checkpoints are too hard for him to choose. Please help Wowo decide whether there exists a sequence of <span class="tex-font-style-bf">real</span> numbers $b_1, \ldots, b_n$ satisfying all the contraints above.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 66\,666$). Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($3 \le n \le 100\,000$).</p><p>The $i$-th of the next $n$ lines contains two integers $x_i^-$, $x_i^+$ ($-10^8\le x_i^-\le x_i^+\le 10^8$) denoting the lower and upper bound of $b_i$. </p><p>The $i$-th of the next $n-1$ lines contains two integers $y_{i+1}^-$, $y_{i+1}^+$ ($-10^8\le y_{i+1}^-\le y_{i+1}^+\le 10^8$) denoting the lower and upper bound of $b_{i+1}-b_i$. </p><p>The $i$-th of the next $n-2$ lines contains two integers $z_{i+2}^-$, $z_{i+2}^+$ ($-10^8\le z_{i+2}^-\le z_{i+2}^+\le 10^8$) denoting the lower and upper bound of $(b_{i+2}-b_{i+1}) - (b_{i+1}-b_i)$. </p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $200\,000$.</p><p>It is guaranteed that relaxing every constraint by $10^{-6}$ (i.e., decrease $x_i^-, y_i^-, z_i^-$ by $10^{-6}$ and increase $x_i^+, y_i^+, z_i^+$ by $10^{-6}$) will not change the answer. </p></div><div class="output-specification"><p>For each test case, output <span class="tex-font-style-tt">YES</span> if a sequence $b_1,\ldots, b_n$ satisfying the constraints exists and <span class="tex-font-style-tt">NO</span> otherwise. The sequence $b_1,\ldots, b_n$ is <span class="tex-font-style-bf">not</span> required.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 66\,666$). Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($3 \le n \le 100\,000$).</p><p>The $i$-th of the next $n$ lines contains two integers $x_i^-$, $x_i^+$ ($-10^8\le x_i^-\le x_i^+\le 10^8$) denoting the lower and upper bound of $b_i$. </p><p>The $i$-th of the next $n-1$ lines contains two integers $y_{i+1}^-$, $y_{i+1}^+$ ($-10^8\le y_{i+1}^-\le y_{i+1}^+\le 10^8$) denoting the lower and upper bound of $b_{i+1}-b_i$. </p><p>The $i$-th of the next $n-2$ lines contains two integers $z_{i+2}^-$, $z_{i+2}^+$ ($-10^8\le z_{i+2}^-\le z_{i+2}^+\le 10^8$) denoting the lower and upper bound of $(b_{i+2}-b_{i+1}) - (b_{i+1}-b_i)$. </p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $200\,000$.</p><p>It is guaranteed that relaxing every constraint by $10^{-6}$ (i.e., decrease $x_i^-, y_i^-, z_i^-$ by $10^{-6}$ and increase $x_i^+, y_i^+, z_i^+$ by $10^{-6}$) will not change the answer. </p>

## Output

<p>For each test case, output <span class="tex-font-style-tt">YES</span> if a sequence $b_1,\ldots, b_n$ satisfying the constraints exists and <span class="tex-font-style-tt">NO</span> otherwise. The sequence $b_1,\ldots, b_n$ is <span class="tex-font-style-bf">not</span> required.</p>

## Samples

```input1
4
3
0 1
0 1
0 1
1 1
1 1
-100 100
3
-967 541
-500 834
-724 669
-858 978
-964 962
-645 705
4
0 0
0 1
0 1
1 1
0 1
0 1
0 1
0 0
0 0
4
0 0
33 34
65 66
100 100
0 100
0 100
0 100
0 0
0 0
```

```output1
NO
YES
YES
NO
```




## Note

<p>In the first test case, all $b_i$'s are in $[0,1]$. Because of the constraints $1=y_2^-\le b_2-b_1\le y_2^+=1$, $b_2-b_1$ must be $1$. So $b_2=1$ and $b_1=0$ must hold. Then by $1=y_3^-\le b_3-b_2\le y_3^+=1$, $b_3$ equals $2$. This contradicts the constraint of $b_3\le 1$. So no solution exists.</p><p>In the second test case, we can let all $b_i$'s be $0$.</p><p>In the third test case, one possible solution is $b_1=0$, $b_2=1/3$, $b_3=2/3$, $b_4=1$. </p>
