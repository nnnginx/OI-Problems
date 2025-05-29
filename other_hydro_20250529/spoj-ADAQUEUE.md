<p>Ada the Ladybug has many things to do. She puts them into her queue. Anyway she is very indecisive, so sometime she uses the top, sometime the back and sometime she decides to reverses it.</p>
<h3>Input</h3>
<p>The first line consists of <strong>1 ¡Ü Q ¡Ü 10<sup>6</sup></strong>, number of queries. Each of them contains one of following commands</p>
<p>back - Print number from back and then erase it</p>
<p>front - Print number from front and then erase it</p>
<p>reverse - Reverses all elements in queue</p>
<p>push_back <strong>N</strong> - Add element <strong>N</strong> to back</p>
<p>toFront <strong>N</strong> - Put element <strong>N</strong> to front</p>
<p>All numbers will be <strong>0 ¡Ü N ¡Ü 100</strong></p>
<h3>Output</h3>
<p>For each back/front query print appropriate number.</p>
<p>If you would get this type of query and the queue would be empty, print "<strong>No job for Ada?</strong>" instead.</p>
<h3>Example Input</h3>
<pre>15
toFront 93
front
back
reverse
back
reverse
toFront 80
push_back 53
push_back 50
front
front
reverse
push_back 66
reverse
front
</pre>
<h3>Example Output</h3>
<pre>93
No job for Ada?
No job for Ada?
80
53
66
</pre>