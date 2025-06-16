<p>In the medieval ages, in the small town of Silent Hill lived a monster named Glutton, which loved terrorising the townsfolk. Many knights have tried to slay it, but none have been able to survive the encounter.</p>
<p>One day, a brave architect called Davis has decided to attack the Glutton. He found out that the monster actually consists of a bunch of <em>parts</em>, interconnected in such a way that each part may <em>control</em>&nbsp;other parts. The Glutton has exactly one part corresponding to its <em>brain</em>; a part not controlled by any other part. Furthermore, the Glutton may have one or more parts that do not control any other part---these correspond to its <em>claws</em>. For every claw there exists <strong>exactly one set of connections</strong>&nbsp;through which the brain (directly or indirectly) controls it. If Davis successfully manages to disconnect the brain from all the claws, the Glutton remains completely harmless.</p>
<p>Davis took advantage of his project skills in order to determine that one may assign a <em>power</em> <em>w</em><em><sub>xy</sub>&nbsp;</em>required to sever&nbsp;each of the Glutton's direct connections <em>x -&gt; y</em>. Davis wishes to invest a <strong>minimal total amount of power</strong>&nbsp;in order to disconnect the brain from all the claws, therefore he is interested in knowing which connections, <strong>left-to-right</strong>, he needs to destroy in order to achieve this. If there are multiple appropriate solutions, Davis would prefer to have the invested power early on be as small as possible, i.e. he would like to know the <strong>lexicographically smallest</strong>&nbsp;appropriate solution.</p>
<p>Blinded by the fame he would attain and the folks' cheers of "Thank you, brave Davis!" should he defeat the Glutton, Davis is too impatient to compute the solution; he has asked you for help.</p>
<h3>Input</h3>
<p>The first line of the standard input contains an integer <em>n</em>, representing the number of the Glutton's parts. The part with ID 1 always represents the brain. Afterwards, a description of all the parts follows in order, starting from the brain, up to the part with ID <em>n</em>, in order, as follows:&nbsp;</p>
<ul>
<li>The first line contains an integer <em>m</em><sub>i</sub>, representing the number of parts directly controlled by the current part.</li>
<li>If <em>m<sub>i </sub>= 0</em>&nbsp;holds, then the current part is a claw.</li>
<li>Otherwise, the second line will contain an array <em>a</em>&nbsp;of <em>m</em><sub>i</sub>&nbsp;integers, representing<strong>&nbsp;</strong>the indices of the parts directly controlled by the current part,&nbsp;<strong>left-to-right</strong>.</li>
<li>The third line will then contain an array <em>w</em>&nbsp;of <em>m</em><sub>i</sub>&nbsp;integers, such that the <em>j</em>-th member of <em>w</em>, <em>w</em><sub>j</sub>, represents the power necessary to destroy the connection through which the current part controls the <em>j</em>-th member of <em>a</em>, <em>a</em><sub>j</sub>.</li>
</ul>
<h3>Output</h3>
<p>Write to the first line of the standard output a single integer representing the minimal total power required for Davis to disable the Glutton. Then, the second line should contain the <em>lexicographically smallest </em>sequence of powers required for severing each of the individual connections, provided in a left-to-right order. Separate individual elements of the sequence with a single space.</p>
<h3>Example</h3>
<pre><strong>Input:<br></strong>7<br>2<br>2 5<br>4 7<br>2<br>3 4<br>2 3<br>0<br>0<br>2<br>6 7<br>1 6<br>0<br>0</pre>
<pre><br><strong>Output:<br></strong>11<br>4 1 6</pre>
<h3>Explanation</h3>
<p>The figures below represent the sample testcase; the left figure represents the Glutton's initial state as provided by the input, and the right figure represents the optimal solution. The brain is denoted by a black background, and the claws are denoted by a red outline. The crossed and dashed connections represent the ones that Davis should destroy. There are <em>two</em>&nbsp;solutions that require the total power of 11; they are, in a left-to-right order, <em>{4, 7}</em>&nbsp;and <em>{4, 1, 6}.</em>&nbsp;We choose the lexicographically smaller out of the two as the final solution.</p>
<p><img src="../../../content/simes:SHILL.png" alt="" width="391" height="129"></p>
<h3>Constraints</h3>
<ul>
<li>2 &lt;= <em>n</em> &lt;= 10<sup>5</sup>;</li>
<li>1 &lt;= <em>w<sub>j</sub></em> &lt;= 10<sup>9</sup>;</li>
<li>The total number of connections will always be <em>n - 1</em>, and for every claw there will exist a unique set of connections linking it to the brain.</li>
</ul>