<p>The Great Plain of Algorithmia plays an extremely important role in the agriculture of the Bandulu Kingdom: this is the only place where barley (Hordeum vulgare), an essential ingredient of beer, can be produced. Unfortunately, it is not possible to grow barley on the full area of the plain, as several nuclear plants have recently been built, and you cannot grow barley near a nuclear plant (since you do not want to produce giant-size, aggressive, man-eating barley-mutants). Your task is to write a program that determines the size of the area that can be used for growing barley.</p>
<p>The Great Plain of Algorithmia is an n * m km<sup>2</sup> rectangle, the coordinates of the four corners being (0, 0),(0, m),(n, 0) and (n, m). There are two types of nuclear plants: small and large. You are not allowed to grow barley within 0.58km of a small nuclear plant or within 1.31km of a large nuclear plant.</p>
<h3>Input</h3>
<p>The input contains several blocks of test cases. Each block begins with a line containing four integers: 1 &lt;= n, m &lt;= 10000 describe the size of the plain, ks &lt;= 100 is the number of small nuclear plants, and kl &lt;= 100 is the number of large nuclear plants. The next ks lines describe the coordinates of the small nuclear plants, each line contains two integers 0 &lt;= x &lt;= n and 0 &lt;= y &lt;= m . The next kl lines describe the large nuclear plants in a similar fashion.</p>
<p>The input is terminated by a block with n = m = ks = kl = 0 .</p>
<h3>Output</h3>
<p>For each test case, you have to output a single line containing the area that can be used for growing barley. This number should be a real value with two digits of precision. To avoid rounding problems, we accept solutions with a maximum of 0.01(positive or negative) error.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
10 10 2 2
2 2
4 4
5 6
1 8
10 10 1 0
5 5
0 0 0 0

<strong>Output:</strong>
87.46
98.94
</pre>