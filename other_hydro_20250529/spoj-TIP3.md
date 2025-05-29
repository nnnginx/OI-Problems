<p>In number theory, Euler's totient (or PHI function), is an arithmetic function that counts the number of positive integers less than or equal to a positive integer N that are relatively prime to this number N.</p>
<p>
That is, if N is a positive integer, then PHI(N) is the number of integers K for which GCD(N, K) = 1 and 1 ¡Ü K ¡Ü N. We denote GCD the Greatest Common Divisor. For example, we have PHI(9)=6.</p>

<p>
Interestingly, PHI(87109)=79180, and it can be seen that 87109 is a permutation of 79180.</p>

<h3>Input</h3>
<p>There is only one number M.
</p>


<h3>Output</h3>
<p>For the given M, you have to print on a single line the value of N, for which 1 &lt; N &lt; M, PHI(N) is a permutation of N and the ratio N/PHI(N) produces a minimum. If there's several answers output the greatest, or if need, "No solution." without quotes.<br>
Leading zeros are not allowed for integers greater than 0.</p>


<h3>Example</h3>

<pre><b>Input:</b>
22

<b>Output:</b>
21


<b>Input:</b>
222

<b>Output:</b>
63


<b>Input:</b>
2222

<b>Output:</b>
291
</pre>

<p><b>Explanations :</b>
For the first case, in the range ]1..22[, the lonely number n for witch phi(n) is in permutations(n) is 21, (we have phi(21)=12). So the answer is obviously 21.<br>
For the second case, in the range ]1..222[, there's two numbers n for witch phi(n) is in permutations(n), we have phi(21)=12 and phi(63)=36. But as 63/36 is equal to 21/12, we're taking the greater : 63.<br>
For the third case, in the range ]1..2222[, there's four numbers n for witch phi(n) is in permutations(n), phi(21)=12, phi(63)=36, phi(291)=192 and phi(502)=250. Within those solutions 291/192 is the minimum, we output 291.</p>


<h3>Constraints</h3>
<pre>1 &lt; M &lt; 10^27
</pre>
<p>If you got TLE, you should consider before <a href="http://www.spoj.com/problems/TIP2/">TIP2</a>. Enjoy.<br>
Warning : don't try to investigate the input number, <a href="http://discuss.spoj.com/t/how-to-add-problem-into-spoj/693/32">judge</a> is strict and interactive ; test case is randomly changing, staying equivalent in difficulty. Please don't use spurious spaces and end your answer with '\n' ; e.g. "21\n" awaited for the sample.<br>
There is many ways to optimize the solution for this problem, to get AC here, you'll need to find many of them.<br>
Time limit allows python3 solutions.<br>
There is different judges, time is the sum of them.
(Edit 2017-02-11, after compiler changes : my Py3 solution ends in 25s, approx 2.5s per file, 10 files.)
</p>