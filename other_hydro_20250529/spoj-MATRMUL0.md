<p>Consider the following C++ code, it constructs n¡Án matrices A,B and vector V from matrix C=A¡ÁB which you need to calculate.</p>
<pre>uint32_t n, i, j, d1, p1, r1, m1, d2, p2, m2, A[n][n], B[n][n];
uint64_t C[n][n], V[n];
<em><span style="color: #ff0000;">//here you need to read n, p1, d1, r1, m1, p2, d2, r2, m2 from input.</span></em>
for (i=0; i&lt;n; ++i)
    for (j=0; j&lt;n; ++j) {
        d1 = d1 * p1 + r1;
        d2 = d2 * p2 + r2;
        A[i][j] = d1 &gt;&gt; (32 - m1);
        B[i][j] = d2 &gt;&gt; (32 - m2);
    }
<em><span style="color: #ff0000;">//here you need to calculate C=A*B</span></em>
for (i=0; i&lt;n; ++i) {
    V[i] = 0;
    for (j=0; j&lt;n; ++j)
        V[i] ^= C[i][j];
}
<em><span style="color: #ff0000;">//here you need to output V[0], V[1], ..., V[n-1], separated by spaces.</span></em>
</pre>
<h3>Input</h3>
<p>You are given integers n, p1, d1, r1, m1, p2, d2, r2, m2, separated by spaces.</p>
<p><span style="font-size: medium;">1¡Ün¡Ü2048</span>, 1¡Üm1,m2¡Ü26, 0¡Üp1,d1,r1,p2,d2,r2&lt;2<sup>32</sup>.</p>
<h3>Output</h3>
<p>You need to output V[0], ..., V[n-1], separated by spaces.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
4 1664525 0 1013904223 26 1664525 1 1013904223 26
<strong>Output:</strong>
3929555766216722 770418013451752 7738542081270672 4286515685761206</pre>
<h3>P.S.</h3>
<p>There are 4 tests with n¡Ö2048. My best solution time ¡ª ~3.2s (~0.8s per test) which is 20 times faster than time limit.</p>
<p>Also try the challenge&nbsp;<a href="../MATRMUL/">MATRMUL</a>, to get AC there your time here should be less than 14s for cubic algorithm and 16s for Strassen's.</p>