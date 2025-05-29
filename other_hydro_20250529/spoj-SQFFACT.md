<p align="justify">Given the positive integers N = p<sub>1</sub> * p<sub>2</sub> * ... * p<sub>k</sub> and M = (p<sub>1</sub>-1) * (p<sub>2</sub>-1) * ... * (p<sub>k</sub>-1),    i.e M = ¦Õ(N) (Euler's totient function),   where k ¡Ý 1, p<sub>i</sub> ¡Ù p<sub>j</sub> for all i¡Ùj with i,j=1,2, ..., k and p<sub>i</sub> is prime number for all i=1,2,...,k, your task is factor n.</p>
<h3>Input</h3>
<p>The first line contains a positive integer T, the number of test cases, where T ¡Ü 100. The following T lines each contains two numbers N and M in this order,  where N &lt; 10<sup>100</sup>.</p>
<h3>Output</h3>
<p>Output T lines, with prime factorization of N according with example.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3
210 48
983 982
14351 14112

<strong>Output:</strong>
210 = 2 * 3 * 5 * 7
983 = 983
14351 = 113 * 127

</pre>