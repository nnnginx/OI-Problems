<p>The well known hardware manufacturing company Processors for Professors is about to release a highly specialized CPU with exceptional functionality in, amongst other areas, number theory. It has, for example, an instruction PFACT that takes one parameter and returns all prime factors of that parameter, with an outstanding execution speed. It has, however, one considerable problem. The scientists at the testing lab has just found out that the PFACT instruction for some special input values freaks out and makes the entire processor explode. Even though this could be an amusing effect, it is not the way it was intended to work. The skilled mathematicians have, by trial and error, found that the explosive numbers all share the same interesting number theoretic properties, which might be of help when troubleshooting. An explosive number is a number x = p0p1p2 . . . pn where all pis are distinct prime numbers such that pi = Api−1 +B for i = 1, 2, . . . , n. n &gt;= 3, p0 = 1. A and B are always integers, and might be different for different explosive numbers. For example, the processor will explode when factorizing the number 4505, because 4505 = 1 · 5 · 17 · 53 and 5 = 3 · 1 + 2, 17 = 3 · 5 + 2 and 53 = 3 · 17 + 2 and the numbers 5, 17 and 53 are all prime numbers. In this case A = 3 and B = 2. You are kindly asked to write a computer program that will aid this company in estimating the impact of the errors, by calculating the amount of explosive numbers that exists within a given range of integers.</p>
<h3>Input</h3>
<p>The input starts with a row containing the number 0 &lt;= N &lt;= 100 of test cases that will follow. For each test case, there will be one row containing two integers, xL and xH separated by a single space. These numbers are such that 0 &lt;= xL &lt;= xH &lt;= 2,000,000,000.</p>
<h3>Output</h3>
<p>For each test case, output the number of explosive numbers that exist in the range xL &lt;= x &lt;= xH.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
4505 4505
0 5000

<strong>Output:</strong>
1
5
</pre>