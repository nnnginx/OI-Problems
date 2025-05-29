<p>
Alice has recently learned to use the Sieve of Eratosthenes, an ancient algorithm for finding all prime numbers up to any given limit. As expected, she was really impressed by it's simplicity and elegancy.
</p>
<p>Now, she has decided to design her own sieve method: The Sieve of Alice, formally defined by the following procedure, which determines the Sieve of Alice up to a given limit N.</p>
<ol>
  <li>Create a list of consecutive integers from N to 2 (N, N-1, N-2, ..., 3, 2). All of those N-1numbers are initially unmarked.</li>
  <li>Initially, let P equal N, and leave this number unmarked.</li>
  <li>Mark all the proper divisors of P (i.e. P remains unmarked).</li>
  <li>Find the largest unmarked number from 2 to P ¨C 1, and now let P equal this number.</li>
  <li>If there were no more unmarked numbers in the list, stop. Otherwise, repeat from step 3.</li>
</ol>

<p>Unfortunately, Alice has not found an useful application for it's Sieve. But she still wants to know, for a given limit N, how many integers will remain unmarked.</p>

<h3>Input</h3>
<p>The first line contains an integer T, the number of test cases (1 ¡Ü T ¡Ü 10^4) . Each of the next T lines contains an integer N (2 ¡Ü N ¡Ü 10^6).</p>

<h3>Output</h3>
<p>Output T lines, one for each test case, containing the required answer.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
3
2
3
5

<strong>Output:</strong>
1
2
3</pre>