<p>In number theory, Euler's totient (or PHI function), is an arithmetic function that counts the number of positive integers less than or equal to a positive integer N that are relatively prime to this number N.</p>
<p>
That is, if N is a positive integer, then PHI(N) is the number of integers K for which GCD(N, K) = 1 and 1 ¡Ü K ¡Ü N. We denote GCD the Greatest Common Divisor. For example, we have PHI(9)=6.</p>

<p>
Interestingly, PHI(87109)=79180, and it can be seen that 87109 is a permutation of 79180.</p>

<h3>Input</h3>
<p>The input begins with the number T of test cases in a single line.<br>
In each of the next T lines there are an integer M.</p>


<h3>Output</h3>
<p>For each given M, you have to print on a single line the value of N, for which 1 &lt; N &lt; M, PHI(N) is a permutation of N and the ratio N/PHI(N) produces a minimum. If there's several answers output the greatest, or if need, "No solution." without quotes.<br>
Leading zeros are not allowed for integers greater than 0.</p>


<h3>Example</h3>

<pre><b>Input:</b>
3
22
222
2222

<b>Output:</b>
21
63
291
</pre>

<p><b>Explanations :</b>
For the first case, in the range ]1..22[, the lonely number n for witch phi(n) is in permutations(n) is 21, (we have phi(21)=12). So the answer is obviously 21.<br>
For the second case, in the range ]1..222[, there's two numbers n for witch phi(n) is in permutations(n), we have phi(21)=12 and phi(63)=36. But as 63/36 is equal to 21/12, we're taking the greater : 63.<br>
For the third case, in the range ]1..2222[, there's four numbers n for witch phi(n) is in permutations(n), phi(21)=12, phi(63)=36, phi(291)=192 and phi(502)=250. Within those solutions 291/192 is the minimum, we output 291.

</p><h3>Constraints</h3>
<pre>1 &lt; T &lt; 10^5
1 &lt; M &lt; 10^7
</pre>
<p>Code size limit is 10kB ; less than 500B of python3 code can get AC under 2s.<br>
After that you may try <a href="http://www.spoj.com/problems/TIP2/">TIP2</a>.<br>
@Speed addicts : my C code ran in 0.02s, and my fastest python3.2 code ran in 1.21s, (0.90s in py2.7) </p>
<p>Edit 2017-02-11, after compiler updates. My old C code ends in 0.00s, my old Python code ends in 0.05s !!!
</p>