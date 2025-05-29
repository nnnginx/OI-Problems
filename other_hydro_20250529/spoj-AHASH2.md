Given a base <strong>B</strong> and a modulo <strong>M</strong>, the polynomial hash of a string <strong>S</strong> consisting of only lowercase letters is defined as below.
<br><br>

Let <strong>S = S<sub>0</sub>S<sub>1</sub>¡­S<sub>N-1</sub></strong> be a string of length <strong>N</strong> containing only the lowercase letters (<strong>a-z</strong>).
<br><br>

<strong>Hash(S) = ¡Æ B<sup>N-i-1</sup> * D(S<sub>i</sub>) % M</strong>
<br><br>

<strong>D(S)</strong> = Lexicographical position of character <strong>S</strong> among the letters <strong>a-z</strong>, indexed from <strong>0</strong>. <strong>D(a) = 0, D(b) = 1, ¡­ , D(z) = 25</strong>.
<br><br>

In other words, first the letters of the string are replaced by numbers (equivalent to their position). This is then considered to be a number in base <strong>B</strong>, and the value of this number in <strong>base 10</strong> modulo <strong>M</strong> is called the polynomial hash of the string.
<br><br>

Calculating the hash of a string using the above method seems easy enough. What about the opposite? You are given a base <strong>B</strong>, a modulo <strong>M</strong>, a positive integer N, and a hash value <strong>H</strong>. Calculate how many strings are there such that their hash is equal to <strong>H</strong>, consisting of only lowercase letters and their length not exceeding <strong>N</strong>. Since the answer can be rather huge, output it modulo <strong>10<sup>9</sup> + 7 (1000000007)</strong>.

<br><br>

<h3>Input</h3>
The first line contains an integer <strong>T</strong>, denoting the number of test cases. Each test case starts with four integers <strong>B, M, N,  Q</strong>. The numbers <strong>B, M, N</strong> denotes the base, modulus and the maximum length of any string as stated above. The number <strong>Q</strong> indicates the number of queries. Each of the next <strong>Q</strong> lines contain a single integer, denoting <strong>H</strong>, the required hash value.

<br><br>

<h3>Constraints</h3>
<strong><li>1 ¡Ü T ¡Ü 150</li></strong>
<strong><li>26 ¡Ü B ¡Ü 30000</li></strong>
<strong><li>1 ¡Ü M, N ¡Ü 30000</li></strong>
<strong><li>1 ¡Ü Q ¡Ü 300</li></strong>
<strong><li>0 ¡Ü H &lt; M</li></strong>
<strong><li>For 95% of the test cases, B, M, N ¡Ü 300</li></strong>

<h3>Output</h3>
For each case, first output a line of the format <strong>Case X:</strong>, where <strong>X</strong> is the case number, starting from <strong>1</strong>. And then, for each query, output the number of different strings with the given hash value modulo <strong>10<sup>9</sup> + 7 (1000000007)</strong> in a single line.
<br><br>
Print a blank line after every test case.

<h3>Sample Input</h3>
<pre>3
26 97 2 3
0
1
96
147 147 147 3
0
10
100
100 110 120 1
35
</pre>

<h3>Sample Output</h3>
<pre>Case 1:
8
8
6

Case 2:
944164777
944164777
0

Case 3:
110169522

</pre>

<br><br>

<h3>Challenge</h3>
You might also enjoy:
<br><br>
<a href="https://www.spoj.com/problems/AHASH/">Anti Hash</a>