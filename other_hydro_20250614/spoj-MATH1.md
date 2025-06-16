<p>You are given n integers a<sub>1</sub>, a<sub>2</sub>,..., a<sub>n</sub> (0&lt;=a<sub>i</sub>&lt;=n). The sum a<sub>1</sub>+ a<sub>2</sub>+...+ a<sub>n</sub> does not exceeded n.
Your task is to find n other integers x<sub>1</sub>, x<sub>2</sub>,..., x<sub>n</sub> (note that x<sub>i</sub> may be negative numbers) satisfying the following conditions:
</p><ul>
<li>(x<sub>i</sub> - x<sub>i+1</sub> + a<sub>i+1</sub> = 0) or (x<sub>i</sub> - x<sub>i+1</sub> + a<sub>i+1</sub> = 1) for i=1..n-1
</li><li>(x<sub>n</sub> - x<sub>1</sub> + a<sub>1</sub> = 0) or (x<sub>n</sub> - x<sub>1</sub> + a<sub>1</sub> = 1) 
</li><li>|x<sub>1</sub>|+|x<sub>2</sub>|+...+|x<sub>n</sub>| is minimized
</li></ul>
<h3>Input</h3>
<p>The first line of the input file contains an integer t representing the number of test cases (t&lt;=20). Then t test cases follow. Each test case has the following form:
</p><ul>
<li>The first line contains n (1&lt;=n&lt;=1000)
</li><li>The second line contains n integers a<sub>1</sub>, a<sub>2</sub>,..., a<sub>n</sub> separated by single spaces
</li></ul>
<h3>Output</h3>
<p>For each test case output a single value: the minimum value of |x<sub>1</sub>|+|x<sub>2</sub>|+...+|x<sub>n</sub>|

</p><h3>Example</h3>

<pre><b>Input:</b>
2
4
2 1 0 0
5
0 1 2 2 0

<b>Output:</b>
1
3

<b>Output Details:</b>
In the former case, the optimal solution is (x<sub>1</sub>=0, x<sub>2</sub>=0, x<sub>3</sub>=0, x<sub>4</sub>=-1)
In the latter case, the optimal solution is (x<sub>1</sub>=-1, x<sub>2</sub>=-1, x<sub>3</sub>=0, x<sub>4</sub>=1, x<sub>5</sub>=0)
</pre>