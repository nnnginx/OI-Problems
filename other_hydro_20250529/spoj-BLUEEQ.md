<p>This morning Blue Mary wrote some equations on a piece of paper and left it on her desk. After solving some problems in SPOJ, she found that her classmate H.L. replaced all characters on the paper with some other ones. H.L. told her he replaced the same characters with the same ones, and different characters with different ones because of his goodness. Now Mary needs your help to get the original equations back.</p>
<p>In Mary's equations, only 13 characters appear:0,1,2,3,4,5,6,7,8,9,+,*,=. There is one and only one "=" in each equation. In H.L.'s equations,only 13 Latin letters appear: a,b,c,d,e,f,g,h,i,j,k,l,m. All the equations are correct in decimal notation. </p>
<p>For example. If Mary wrote down 2+29=31, H.L. replaced 2 with i, + with l, 9 with k, = with e, 3 with m and 1 with a, we got ilikema . </p>
<h3>Input</h3>
<p>The first line contains a single integer t.t blocks follow.</p>
<p>To every block,the first line contains a single integer n(1&lt;=n&lt;=1000). n lines follow,each contains a string whose length is more than 4 and less than 12.The string contains only a-m and doesn't contain any whitespaces.</p>
<p>At least 90% of test cases satisfy that n&lt;=5.</p>
<p>At least 80% of test cases satisfy that n&lt;=2.</p>
<p>In at least 70% of test cases, there are at most 5 different characters in all the equations.</p>
<h3>Output</h3>
<p>If there doesn't exist n equations that can be translated to H.L.'s equations,print a line contains the word <em> noway </em>.Otherwise you should output all the corresponding relations that can be fixed in lexicographic order,see the example. </p>
<h3>Example</h3>
<pre><b>Input</b>
1
2
abcdec
cdefe

<b>Output</b>
a6
b*
d=
f+
</pre>
<h3>hint</h3>
<p>The two strings can be translated to the following equations possibly:</p>
<pre>6*2=12 2=1+1
6*4=24 4=2+2
6*8=48 8=4+4
</pre>
<p>So the corresponding relations above can be fixed,others can not.</p>