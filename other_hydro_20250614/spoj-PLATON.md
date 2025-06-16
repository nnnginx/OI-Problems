<p>Platon and Socrates one day decided to play a new game. They asked their friend to think of two numbers between 1 and 5000, not equal. Then they asked him to tell the product to Platon and the sum to Socrates. After that they tried to figure out what these numbers are. They played a lot of times but none of them could guess these numbers. Finally they made it!! Here is the dialogue:
</p><div align="left">
<ul>
<li>[P] : I don't know the answer.
</li><li>[S] : I knew you wouldn't know, I don't know it either.
</li><li>[P] : Now I know it.
</li><li>[S] : I know it too.
</li></ul>

Your task is to find all pairs Platon and Socrates could have been thinking about. Numbers are limited to the given range.
</div>
<p></p>
<h3>Input</h3>
<p>Input starts with a single integer t, the number of test cases (t&lt;=2000). t test cases follow. Each test case consists of one line containing two integers <var>l r</var> seperated by a single space, denoting the range of numbers ( <var>1&lt;= l &lt; r &lt;=5000</var>, <var>r-l &lt; 200</var> ). 


</p><h3>Output</h3>
<p>For the i-th test case output a line with the text <var>case i</var>. In the next line print <var>n</var> - number of pairs from range <var>(l,r)</var>. Then exactly <var>n</var> lines follow with two numbers seperated by single space. The first number is not greater than the second. Pairs are printed in increasing sum order.
</p><h3>Example</h3>

<pre><b>Input</b>
2
1 10
2 8

<b>Output</b>
case 1
0
case 2
0
</pre>