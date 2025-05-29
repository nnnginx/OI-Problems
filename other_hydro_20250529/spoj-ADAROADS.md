<p>As you might already know, Ada the Ladybug is a farmer. She grows many fruits and vegetables. She has to take care of them so she builds many roads between them. She also doesn't want to keep unnecessary roads so after builting a road she cleans the rest of roads so her road-system doesn't contain any needless cycles. Each road has some maintenance cost and she always keeps roads in such ways that the total cost is minimized.</p>
<h3>Input</h3>
<p>The first line of input containts  <strong>1 ¡Ü N ¡Ü 2*10<sup>5</sup>, 0 ¡Ü M ¡Ü     5*10<sup>5</sup></strong>, the number of vegetables and the number of roads built by Ada.</p>
<p>The next <strong> M </strong> lines contains three integers <strong>a, b, c: 0 ¡Ü a, b     &lt; N, 0 ¡Ü c ¡Ü 10<sup>9</sup>, a ¡Ù b</strong>, the vegetables connected by road and its maintanance cost.</p>
<p>To simulate the "real-time", <strong>a, b, c</strong> will be on input as <strong>a ¨’     l, b ¨’ l, c ¨’ l</strong>, where <strong>l</strong> is the last answer (start as 0) and operation stands for binary XOR.</p>
<h3>Output</h3>
<p>For each new road print the number actual best sum of maintenance costs.</p>
<h3>Example Input</h3>
<pre>5 5
4 3 6
6 7 4
8 9 10
8 12 9
8 10 11
</pre>
<h3>Example Output</h3>
<pre>6
8
8
9
5
</pre>
<h3>Real queries</h3>
<pre>REAL QUERY: 4 3 6
REAL QUERY: 0 1 2
REAL QUERY: 0 1 2
REAL QUERY: 0 4 1
REAL QUERY: 1 3 2
</pre>
<h3>Example Input 2</h3>
<pre>6 9
3 2 7
4 5 13
2 6 3
11 10 14
17 18 18
16 23 26
19 18 17
18 19 21
14 13 12
</pre>
<h3>Example Output 2</h3>
<pre>7
7
11
16
18
18
16
14
11
</pre>
<h3>Real queries 2</h3>
<pre>REAL QUERY: 3 2 7
REAL QUERY: 3 2 10
REAL QUERY: 5 1 4
REAL QUERY: 0 1 5
REAL QUERY: 1 2 2
REAL QUERY: 2 5 8
REAL QUERY: 1 0 3
REAL QUERY: 2 3 5
REAL QUERY: 0 3 2
</pre>
<h3>Example Input 3</h3>
<pre>3 4
0 1 8
8 10 13
15 13 4
13 12 8
</pre>
<h3>Example Output 3</h3>
<pre>8
13
13
10
</pre>
<h3>Example Input 4</h3>
<pre>6 7
4 3 3
3 6 4
14 9 13
8 15 14
11 13 9
17 16 20
13 14 6
</pre>
<h3>Example Output 4</h3>
<pre>3
10
10
14
21
15
24
</pre>
<h3>Example Input 5</h3>
<pre>7 11
3 0 997179154
997179152 997179154 204554238
1926119418 1926119416 1370896084
2521188650 2521188654 3204670819
3213587831 3213587825 2592574673
3142795976 3142795983 3067341340
3369331620 3369331617 3266995941
3544021221 3544021220 3341161807
2952422819 2952422823 3068368185
2952422818 2952422823 3137316850
2952422817 2952422819 2934379046
</pre>
<h3>Example Output 5</h3>
<pre>997179154
1926119422
2521188648
3213587827
3142795978
3369331616
3544021221
2952422819
2952422819
2952422819
2349523846
</pre>