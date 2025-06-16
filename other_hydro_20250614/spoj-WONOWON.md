<p>There is a little village in northern Canada called Wonowon, its name coming from the fact that it is located at Mile 101 of the Alaska Highway. While passing through this village, a wandering mathematician had an idea for a new type of number, which he called a wonowon number. He defined a wonowon number as a number whose decimal digits start and end with 1, and alternate between 0 and 1. Thus, the first four wonowon numbers are 101, 10101, 1010101, 101010101.</p>
<p>Neither 2 nor 5 can divide any wonowon number, but it is conjectured that every other prime number divides some wonowon number. For example, 3 divides 10101 (i.e. 3×3367), 7 divides 10101 (i.e. 7×1443), 11 divides 101010101010101010101 (i.e. 11 × 9182736455463728191).</p>
<p>Assume throughout that this conjecture is true, and let W(p) denote the number of digits in the smallest wonowon number divisible by p. Thus, for example, W(3) = 5, W(7) = 5, W(11) = 21, W(13) = 5, W(17) = 15, W(19) = 17.</p>
<p>It has been found experimentally that for many primes p, W(p) = p − 2 (as in the case for p = 7, 17, 19). Thus, your task is to write a program which reads an integer n and outputs the number of primes for which W(p) = p − 2. Note that p cannot be 2 nor 5, and p is a prime number less-than or equal to n.</p>
<h3>Input</h3>
<p>The input consists of a single integer 3 ≤ n ≤ 10000.</p>
<h3>Output</h3>
<p>The output should consist of a single integer representing the number of primes p for which W(p) = p − 2.</p>
<h3><span style="font-size: 1.17em;">Example One</span></h3>
<pre><strong>Input:</strong>
20</pre>
<pre><strong>Output:</strong>
3</pre>
<h3>Example Two</h3>
<pre><strong>Input:</strong>
100</pre>
<pre><strong>Output:</strong>
14</pre>