<p>Consider the hash function h(y) = a*y + b (mod m) which maps each
integer to some integer between 0 and m-1.  You are given
x,n,c,d and are curious how many of the hash values
h(x),h(x+1),...,h(x+n) land in the interval [c,d].

</p><h3>Input</h3>
<p>The first line contains a positive integer t, the number of test
cases (1 ¡Ü t ¡Ü 10^5).  t lines then follow, where the ith
line gives the values a,b,x,n,c,d,m,
space-separated, for the ith test case.  All given values are
non-negative.  Also,
1 ¡Ü m ¡Ü 10<sup>15</sup>, c ¡Ü d &lt; m, a,b &lt; m, x+n ¡Ü
10<sup>15</sup>, and a*(x+n) + b ¡Ü 10<sup>15</sup>.

</p><h3>Output</h3>
<p>For each test case in order output the number of i, 0 ¡Ü i ¡Ü n,
such that c ¡Ü a*(x+i) + b (mod m) ¡Ü d in that test case,
followed by a newline.

</p><h3>Example</h3>

<pre><b>Input:</b>
2
2 3 1 3 0 1 7
1 0 0 8 0 8 9

<b>Output:</b>
1
9
</pre>