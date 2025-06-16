<p>Progressive climate change has forced the Byteburg authorities to build a huge lightning conductor     that would protect all the buildings within the city.     These buildings form a row along a single street, and are numbered from <strong>1</strong> to <strong>n</strong>.</p>
<p>The heights of the buildings and the lightning conductor are non-negative integers. Byteburg's limited funds allow construction of only a single lightning conductor.     Moreover, as you would expect, the higher it will be, the more expensive.</p>
<p>The lightning conductor of height <strong>p</strong> located on the roof of the building <strong>i</strong> (of height <strong>hi</strong>)     protects the building <strong>j</strong> (of height <strong>hj</strong>) if the following inequality holds:</p>
<p>hj &lt;= hi + p - sqrt(abs(i-j))</p>
<p>where <strong>|i-j|</strong> denotes the absolute value of the difference between <strong>i</strong> and <strong>j</strong>.</p>
<p>Byteasar, the mayor of Byteburg, asks your help.     Write a program that, for every building, determines the minimum height of a lightning conductor that would protect all the buildings if it were put     on top of the building <strong>i</strong>.</p>
<h2>Input</h2>
<p>In the first line of the standard input there is a single integer     <strong>n</strong> (<strong>1 &lt;= n &lt;= 500,000</strong>) that denotes the number of buildings in Byteburg.     Each of the following <strong>n</strong> lines holds a single integer <strong>hi</strong> (<strong>1 &lt;= hi &lt;= 1,000,000,000</strong>)     that denotes the height of the <strong>i</strong>-th building.</p>
<h2>Output</h2>
<p>Your program should print out exactly <strong>n</strong> lines to the standard output.     The <strong>i</strong>-th line should give a non-negative integer <strong>pi</strong> denoting the minimum     height of the lightning conductor on the <strong>i</strong>-th building.</p>
<h2>Example</h2>
<p>For the input data:</p>
<pre>6
5
3
2
4
2
4</pre>
<p>the correct result is:</p>
<pre>2
3
5
3
5
4</pre>