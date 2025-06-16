<p>Peter has an amoeba farm with pretty much unlimited amoebae. After years of research, Peter created a device to convert some amoebae to super amoebae. However, his device can only be used once. Every day, a super amoeba will split into M super amoebae (2 <span style="text-decoration: underline;">&lt;</span>&nbsp;M <span style="text-decoration: underline;">&lt;</span>&nbsp;100000).</p>
<p>Now, Peter plan his amoeba selling business. Initially, Peter converts X amoebae to super amoebae (X <span style="text-decoration: underline;">&gt;</span>&nbsp;1). Every day after the amoebae split, Peter will take Y super amoebae for sale (Y <span style="text-decoration: underline;">&gt;</span>&nbsp;1). After N days, Peter want all of his amoebae to be completely sold out (1 <span style="text-decoration: underline;">&lt;</span>&nbsp;N <span style="text-decoration: underline;">&lt;</span>&nbsp;100000). Since the energy needed to convert amoebae is quite massive, X must be as small as possible. Help peter plan his business!</p>
<h3>Input</h3>
<p>First line is T, number of test cases (T <span style="text-decoration: underline;">&lt;</span>&nbsp;100000). Next T lines each contains M and N separated by space.</p>
<h3>Output</h3>
<p>For each case, output X and Y separated by space. Since X and Y can be very large, output them with modulo 1000000007.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1<br>4 3

<strong>Output:</strong>
21 64</pre>
<h3>Explanation</h3>
<p>Initially, Peter has 21 super amoebae.<br>After day 1, there are 4 x 21 - 64 = 20 super amoebae<br>After day 2, there are 4 x 20 - 64 = 16 super amoebae<br>After day 3, there are 4 x 16 - 64 = 0 super amoeba<br>All the super amoebae are sold out after the 3rd day just as planned.</p>