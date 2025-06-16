<p>Erdős Pál and John Selfridge classified prime numbers in this way: for a prime <strong>p</strong>, if the largest prime factor of <strong>p-1</strong> is <strong>2</strong> or <strong>3</strong>, then <strong>p</strong> is in class one.  Otherwise, <strong>p</strong> is in class <strong>c+1</strong> where <strong>c</strong> is the largest of the classes of the prime factors of <strong>p-1</strong>. We put <strong>p=2</strong> in class one.  For example, <strong>p=89</strong> is in class three, because <strong>p-1=2^3*11</strong> and here <strong>2</strong> is in class one, but <strong>11</strong> is in class two (because <strong>11-1=2*5</strong> and here <strong>2</strong> and <strong>5</strong> are in class one). Your task is to count the number of primes in each class up to class thirteen for a given (closed) interval.</p>
<h3>Input</h3>
<p>The first line contains the number of test cases <em>T</em>, where <em>T≤1000</em>. Each of the following <em>T</em> lines contains two integers <strong>a,b</strong> where&nbsp;<em><strong>0≤a≤b≤50000000</strong></em>. <span style="color: #000020; font-size: 13px; text-align: justify; background-color: #f6f9e0;">There are 4 input sets for 10 points.</span></p>
<h3>Output</h3>
<p>Output the case number, followed by the distribution of the primes in each class up to class <strong>13</strong> in the (closed) interval <em>[a,b]</em>. See the sample input/output for the correct format!</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3
2 100
23 23
0 50000000

<strong>Output:</strong>
Case 1:
There are 10 primes in class 1.
There are 9 primes in class 2.
There are 5 primes in class 3.
There are 1 primes in class 4.
There are 0 primes in class 5.
There are 0 primes in class 6.
There are 0 primes in class 7.
There are 0 primes in class 8.
There are 0 primes in class 9.
There are 0 primes in class 10.
There are 0 primes in class 11.
There are 0 primes in class 12.
There are 0 primes in class 13.

Case 2:
There are 0 primes in class 1.
There are 0 primes in class 2.
There are 1 primes in class 3.
There are 0 primes in class 4.
There are 0 primes in class 5.
There are 0 primes in class 6.
There are 0 primes in class 7.
There are 0 primes in class 8.
There are 0 primes in class 9.
There are 0 primes in class 10.
There are 0 primes in class 11.
There are 0 primes in class 12.
There are 0 primes in class 13.

Case 3:
There are 54 primes in class 1.
There are 14196 primes in class 2.
There are 364182 primes in class 3.
There are 1029984 primes in class 4.
There are 939493 primes in class 5.
There are 458831 primes in class 6.
There are 150902 primes in class 7.
There are 34878 primes in class 8.
There are 7085 primes in class 9.
There are 1310 primes in class 10.
There are 203 primes in class 11.
There are 15 primes in class 12.
There are 1 primes in class 13.
</pre>
<p><strong>Warning: A naive algorithm will probably solve only the first input set. </strong></p>