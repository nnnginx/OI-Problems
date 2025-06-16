<p>Trey Parker and Matt Stone, the creators of ¡°South Park¡± are having some problems handling their fans. The number of fans is so huge that can¡¯t even count them properly. So they hired ¡°N¡± employees for counting the fans. All the ¡°N¡± employees had their own separate offices and they were located in a straight line with positions numbered as 1, 2, 3 ¡­ up to N. Fans can come to the office of any employee at any time and tell them how they feel about the show and if they are lucky enough, they may get to meet Trey Parker and Matt Stone.</p>
<p>All the employees keep on updating Trey and Matt about the number of fans currently in their offices, so at each moment, they will have a list of ¡°N¡± positions and the number of fans in each of these positions. Trey and Matt suddenly start taking a walk from office at position ¡°A¡± to position ¡°B¡± to meet their fans, but before they start walking they want to know the sum of all the fans in the offices from position ¡°A¡± to ¡°B¡±. But counting them one by one is taking a lot of time, so now they hired you, an awesome software engineer to do this task. Your task is to find the sum of all the fans present in the offices between positions ¡°A¡± to ¡°B¡± ("A" and "B" inclusive). Let¡¯s see if you could do it fast enough.</p>
<h3>Input</h3>
<p>The first line of Input contains two integers ¡°N¡± and ¡°Q¡±. ¡°N¡± is the no. of employees hired by Trey and Matt. ¡°Q¡± is the no. of queries to be followed.</p>
<p>Each of the next ¡°Q¡± lines contain a query. A query can be of two types:</p>
<p>¡°add P F¡± ¨C this means that ¡°F¡± no. of fans came to the office at Position ¡°P¡±</p>
<p>¡°find A B¡± ¨C this means that Trey and Matt wants to know the sum of fans present at offices at positions ¡°A¡± to ¡°B¡±</p>
<h3>Output</h3>
<p>For each query of the type ¡°find A B¡±, output the sum of fans present at offices at positions ¡°A¡± to ¡°B¡± in a different line.</p>
<h3>Constraints</h3>
<p>1 &lt;= N &lt;= 10^6</p>
<p>1 &lt;= Q &lt;= 10^5</p>
<p>1 &lt;= A &lt; B &lt;= N</p>
<p>1 &lt;= P &lt;=N</p>
<p>1 &lt;= F &lt;= 10^4</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
</pre>
<pre>10 10</pre>
<pre>find 1 5
</pre>
<pre>add 5 8</pre>
<pre>add 6 2</pre>
<pre>find 4 5</pre>
<pre>find 4 6</pre>
<pre>add 2 4</pre>
<pre>find 2 6</pre>
<pre>add 6 7</pre>
<pre>find 1 6</pre>
<pre>find 7 10
<strong><br></strong></pre>
<pre><strong>Output:</strong></pre>
<pre>0
</pre>
<pre>8</pre>
<pre>10</pre>
<pre>14</pre>
<pre>21</pre>
<pre>0</pre>