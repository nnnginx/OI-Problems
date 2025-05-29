<p>Maggu is a weird guy. Whenever he gets bored, he starts playing weird games. As he is an odd boy, he likes to play only with arrays of even length n. Maggu cannot play with large numbers, so he will do all the operations modulo 10^9 + 7.
</p>

<p>He likes performing "weird operations" on the array very much. A Weird Operation#1 on an array seq[] is defined as follows:</p>

<pre>tempSeq[n] ; //is a temporary array
for (i = 0; i &lt; n; i++) &nbsp;{
    int cnt = 0;
    for (cnt = 0; cnt &lt; k; cnt++) {
        int j = (i + cnt) % n;
        if (cnt % 2 == 0) tempSeq[i] += seq[j];
        else tempSeq[i] -= seq[j];
    }
}
for (int i = 0; i &lt; n; i++) seq[i] = tempSeq[i];</pre>

<p>Weird operation#2 is even more cooler than this. In this operation, he swaps the adjacant entries of the array.</p>

<p>Pseudo code is as follows:</p>
<pre>for (int i = 0; i &lt; n; i += 2) swap (seq[i], seq[i + 1]);</pre>

<p>A "Super Weird operation" is applying weird operation #1 followed by weird operation #2 on the array seq[]. He wants to apply this operation m times and desires to know the final contents of the seq.</p>
<p>He is bored of playing this game, So he asks you to find out the final content of the seq.</p>

<h3>Input</h3>
<p>
First line contains number of test cases: T (1 &lt;= T &lt;= 100).</p>
<p>For each test case, first line contains three space seperated n, k, m (1 &lt;= n &lt;= 50, 1 &lt;= k &lt;= n, 1 &lt;= m &lt;= 10^9). n is always even.</p><p>The next line contains n space separated integers seq[i](starting from 0), -10^9 &lt;= seq[i] &lt;= 10^9.</p>

<h3>Output</h3>
<p>
For each test case, output n space separated integers where ith element represents seq[i] after m "Super Weird Operations".</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
1
4 3 1
2 4 -3 5

<strong>Output:</strong>
12 1000000002 7 1000000001</pre>