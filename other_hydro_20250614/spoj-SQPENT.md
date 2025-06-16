<p>Garima is a Geometry enthusiast, she loves solving geometry puzzles and creating new puzzles by herself. One fine day she was trying to arrange some "dots" (.) in a form of square.</p>
<p>As shown in figure below:</p>
<p><img title="Square Numbers" src="./24443/file/fUF7KRt9.png" alt="Square Numbers created using dots" width="640" height="152"></p>
<p>&nbsp;</p>
<p>She observes that the number of dots needed to create a square of size 'n' is n*n i.e. 1, 4, 9, 16 , 25, and so on.</p>
<p>She wanted to make larger polygons with these dots, so she started making pentagons, as shown in figure below.</p>
<p><img title="Pentagonal Numbers" src="./24443/file/UMQdO5qa.png" alt="Pentagonal Numbers created using dots" width="640" height="182"></p>
<p>&nbsp;</p>
<p>Being a bright Mathematics student, she is quick to figure out that to create pentagon of size 'n' she needs (3*n*n - n)/2 dots i.e. 1, 5, 12, 22, 35, and so on.&nbsp;</p>
<p>Now she wonders, if she can ever use the same number of dots to make a square as well as a pentagon, of different sizes of course.</p>
<p>She tries a few numbers, but cannot think of any number other than 1, which can make both square and pentagon.</p>
<p>She tried a lot of numbers, now she thinks, such numbers might be too big, so she asks her programmer friend to write a program to find such numbers which can arranged as both square and pentagon.</p>
<p>Her programmer friend, understanding that these numbers can be big, promises her to find such numbers modulo 3367900313, a random big enough prime number.</p>
<p><span style="white-space: pre;">Assume that you are her friend, now help her to find these numbers!</span></p>
<h3>Input</h3>
<p>The first line contains a single positive integer 't', describing the number of test cases.</p>
<p>Next 't' lines contains postive integer 'r', such that 1 &lt;= r &lt;= 2500 . Also, 1&lt;= t &lt;= 100.</p>
<h3>Output</h3>
<p>For each test case, find out r<sup>th</sup>&nbsp;number, when considered in sorted ascending order, which can be arranged as a pentagon as well as a square, as described in the problem</p>
<p>Print a single line corresponding to each test case. Since the answers can be long, so don't forget to take modulo 3367900313</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
</pre>
<pre>2</pre>
<pre>1</pre>
<pre>2
</pre>
<pre><strong>Output:</strong>
</pre>
<pre>1</pre>
<pre>9801</pre>
<pre><strong>Explanation:</strong></pre>
<pre>The first such number is 1, after that next number is 9801 which can make a square of size 99, as 99 * 99 = 9801 and </pre>
<pre>it can make a pentagon of size 81, as (3*81*81-81)/2 = 9801</pre>