<p>
A number is&nbsp;<strong>Almost-K-Prime</strong>&nbsp;if it has exactly<strong>&nbsp;K</strong>&nbsp;prime numbers (not necessarily distinct) in its prime factorization. For example, 12 = 2 * 2 * 3 is an&nbsp;Almost-3-Prime&nbsp;and 32 = 2 * 2 * 2 * 2 * 2 is an&nbsp;Almost-5-Prime&nbsp;number.&nbsp;A number&nbsp;<strong>X</strong>&nbsp;is called&nbsp;<strong>Almost-K-First-P-Prime</strong>&nbsp;if it satisfies the following criterions:</p>

<ol>
  <li>X&nbsp;is an&nbsp;Almost-K-Prime&nbsp;and</li>
  <li>X&nbsp;has&nbsp;<strong>all and only</strong>&nbsp;the first&nbsp;P (P ¡Ü K)&nbsp;primes in its prime factorization.</li>
</ol>
<p>For example, if&nbsp;K=3&nbsp;and&nbsp;P=2, the numbers 18 = 2 * 3 * 3 and 12 = 2 * 2 * 3 satisfy the above criterions. And 630 = 2 * 3 * 3 * 5 * 7 is an example of&nbsp;Almost-5-First-4-Pime.</p>
<p>For a given&nbsp;K&nbsp;and&nbsp;P, your task is to calculate the summation of&nbsp;<strong>¦µ(X)</strong>&nbsp;for all integers&nbsp;X&nbsp;such that&nbsp;X&nbsp;is an&nbsp;Almost-K-First-P-Prime.</p>
<p>In mathematics&nbsp;<strong>¦µ(X)</strong>&nbsp;means the number of relatively prime numbers with respect to&nbsp;X&nbsp;which are smaller than&nbsp;X. Two numbers are relatively prime if their GCD (Greatest Common Divisor) is 1. For example,&nbsp;¦µ(12) = 4, because the numbers that are relatively prime to 12 are: 1, 5, 7, 11.</p>

<h3>Input</h3>
<p>Input starts with an integer&nbsp;<strong>T (¡Ü 10000)</strong>, denoting the number of test cases.</p>
<p>Each case starts with a line containing two integers&nbsp;<strong>K (1 ¡Ü K ¡Ü 500)</strong>&nbsp;and&nbsp;<strong>P (1 ¡Ü P ¡Ü K)</strong>.</p>

<h3>Output</h3>
<p>For each case, print the case number and the result modulo&nbsp;<strong>1000000007</strong>.</p>

<h3>Example</h3>
<pre><b>Input:</b>
3
3 2
5 4
99 45

<b>Output:</b>
Case 1: 10
Case 2: 816
Case 3: 49939643</pre>