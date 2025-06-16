<p>Topuch is the name of the brand new bubble tea shop just opened on your street. Just for a bubble tea lover like you :3</p>
<p>Touch and Top, the owners of the shop, think that the tea that comes after and have less sweetness than the previous one is unique. So they would consider the pair of tea that is unique as having the uniqueness value of 1. You've just finished reading the shop description and suddenly, a cute girl in pink come up to you and ask you if you can calculate the uniqueness of the range of the tea sequence for her. You have to help help her.... :3</p>
<p>The uniqueness in range <strong>L...R</strong> is defined by the number of the pair of <strong>(i,j) L&lt;=i &lt;= j&lt;=R</strong> that the sweetness of tea at <strong>i</strong> is higher than the one at <strong>j</strong>.</p>
<h3>Input</h3>
<p>The first line contains a single number <strong>N</strong> denoting the size of the tea sequence. <strong>(1 &lt;= N &lt;= 5000)</strong></p>
<p>The second line contains <strong>N</strong> numbers; <strong>Ai</strong> denoting the sweetness of each tea. <strong>(1 &lt;= Ai &lt;= 1e9) (1 &lt;= i&nbsp; &lt;= N)</strong></p>
<p>The third line contains a single number <strong>M</strong> denoting the number of question the girl want to ask you. <strong>(1 &lt;= M &lt;= 1e6)</strong></p>
<p>The next <strong>M</strong> lines each contain two numbers; <strong>L R</strong> meaning that the question asks about the sum of uniqueness of the all tea that is in range index <strong>L</strong> to <strong>R</strong>. <strong>(1 &lt;= L &lt;= R &lt;= N)</strong></p>
<h3>Output</h3>
<p><strong>M</strong> lines each contain a single number; <strong>Bj</strong> denoting the answer for the question <strong>j</strong>.&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
8 
3 5 6 2 4 5 7 1
5
1 3
2 4
2 5
1 8
4 7
</pre>
<pre><strong>Output:</strong>
0
2
4
13<br>0</pre>