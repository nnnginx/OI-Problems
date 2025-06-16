<p>You are creating a new soical network for dogs. Wow. The dogs don't have many possibilities for interacting with your website, but they can bark how many friends they want. E.g. if a dog wants to have much 8 friends it will bark 8 times, and if it doesn't want any friends, it'll just stay quiet.</p>
<p>After spending a good year of your life collecting these barks, you are finally ready to assign a friend list for each dog. The only problem is: You are not sure whether it is actually possible. Thus before you proceed you would like to write a program, that given a list of <strong>N</strong> wishes <strong>w<sub>i</sub></strong>, outputs <strong>HAPPY</strong> if it is possible to make a friend list for each dog <strong>i</strong> of length <strong>w<sub>i</sub></strong>, or <strong>SAD</strong> if some dog will have to get more or fewer friends than it wished for.</p>
<p>Notice: Being friends is considered a reflexive relation.</p>
<h3>Input</h3>
<p>The first line will contain a single integer <strong>T</strong> - the number of test cases to process.</p>
<p>Because of I/O constraints, the sequence of wishes is not given explicitly. Each of the <strong>T</strong> lines will consist of 5 integers <strong>N</strong>, <strong>a</strong>, <strong>b</strong>, <strong>c</strong>, <strong>m</strong> in the range <strong>[0, 10^7]</strong> (except <strong>m</strong> which is in <strong>[1, 10^7]</strong>). These integers describe the sequence</p>
<pre>x<sub>0</sub> = 0<br>x<sub>i+1</sub> = (a*x<sub>i </sub>+ b) % m</pre>
<p>The sequence of wishes is <strong>w<sub>i</sub></strong>&nbsp;= <strong>x<sub>i</sub></strong> + <strong>c</strong>.</p>
<h3>Output</h3>
<p>Write the answer - <strong>HAPPY</strong> or <strong>SAD</strong> - for each test case on a separate line.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3
3 2 1 0 2
5 1 1 0 5
6 1 1 1 3

<strong>Output:</strong>
HAPPY<br>SAD<br>HAPPY</pre>
<h3>Explanation</h3>
<p>In the first case we get the wishes "0 1 1", and we &nbsp;can make dog 2 and 3 be friends.</p>
<p>In the second case we get the wishes "0 1 2 3 4". No assignment that works, since dog 5 would have to be friends with everyone, but dog 1 doesn't want that.</p>
<p>In the third case we get the wishes "1 2 3 1 2 3".</p>