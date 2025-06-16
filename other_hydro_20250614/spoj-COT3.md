<p>Alice and Bob are playing a game on a tree of n nodes.Each node is either black or white initially.</p>
<p>They take turns to do the following operation:<br>Choose a white node v from the current tree;<br>Color all white nodes on Path(1,v) to black.</p>
<p>The player who takes the last turn wins.</p>
<p>Now Alice takes the first turn.Help her&nbsp;find out if she can win when they both use optimal strategy.</p>
<h3>Input</h3>
<p>The first line of input contains a integer n representing the number of nodes in the tree. 1&lt;=n&lt;=100000</p>
<p>The second line contains n intergers c1,c2,..cn.0&lt;=ci&lt;=1.<br>ci=0 means the ith node is white initially and ci=1 means black.</p>
<p>Next n-1 lines describes n-1 edges in the tree.Each line contains two integers u and v,means there is a edge connecting u and v.&nbsp;</p>
<h3>Output</h3>
<p>If Alice can't win print -1.</p>
<p>Otherwise determine all the nodes she can choose in the first turn in order to win.Print them in ascending order.</p>
<h3>Example</h3>
<pre><strong>Input#1:</strong>
8<br>1 1 0 1 0 0 1 0<br>1 2<br>1 3<br>2 6<br>3 4<br>3 5<br>5 7<br>7 8&nbsp;</pre>
<pre><strong>Output#1:</strong>
5</pre>
<pre><strong>Input#2:<br></strong>20<br>1 1 1 0 1 1 1 0 1 0 0 0 1 0 1 0 0 0 0 0<br>1 2<br>2 3<br>2 4<br>1 5<br>1 6<br>5 7<br>5 8<br>2 9<br>8 10<br>1 11<br>1 12<br>9 13<br>6 14<br>14 15<br>7 16<br>11 17<br>2 18<br>7 19<br>12 20&nbsp;</pre>
<pre><strong>Output#2<br></strong>8<br>11<br>12&nbsp;</pre>