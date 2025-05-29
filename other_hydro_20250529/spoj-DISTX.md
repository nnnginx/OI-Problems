<p>In this task let's consider distance between two positive integers defined as below.</p>
<p>Single  operation is : multiplying some number by prime number or dividing some  number by prime number ( we can divide only when remainder is equal to 0  )</p>
<p>Distance d between two numbers a,b is minimum number operations to convert one number to another.</p>
<p>For example d(69,42)=3</p>
<p>This distance is very similiar to well-known term "distance" in real human life:</p>
<p>d(a,a)=0 , distance number to itself is 0</p>
<p>d(a,b)=d(b,a) distance from a-&gt;b is equal to b-&gt;a</p>
<p>d(a,b)+d(b,c)&gt;=d(a,c) triangle equation is true too</p>
<p>With given n number you have to determine for each i-th of those numbers closest number aj from set that</p>
<p>i!=j and if there is many numbers with equal, smallest distance, you have to pick number with smallest index</p>
<h3>Input</h3>
<p>In first line - number n &lt;=10^5.</p>
<p>In next n lines - i-th number. Every number is not greater than 10^6</p>
<h3>Output</h3>
<p>You have to output n lines.</p>
<p>I-th line should contain index of closest number ( if there is many answers, please output smallest index )</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
6<br>1<br>2<br>3<br>4<br>5<br>6<br><strong>Output:</strong>
2<br>1<br>1<br>2<br>1<br>2 <br></pre>