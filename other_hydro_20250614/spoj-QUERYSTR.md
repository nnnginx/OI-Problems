<p><br>McFn interesed in string problem recently.He found a interesing function and he felt he could use this function to invent a new match algorithm.<br><br>For a string S [1 ... n] and i ¡Ê [1, n], define F (i) is the length of the longest common suffix of S and S [1 ... i]. <br>For example, for the string S [1 ... 11] = zaaxbaacbaa, then F (1) = 0, F (2) = 1, F (3) = 2 (note that S [1 ... 3] = zaa), F (4) = 0, ... ... F (10) = 1, F (11) = 11; <br>For the string S [1 ... n], i ¡Ê [1, n], S [i ... n] is its suffix;</p>
<h3>Input</h3>
<p>The first line is a integer T.the number of test cases<br>for each test case<br>The first line is a string S, composed of only lowercase letters,&nbsp; len (s) is the length of s,&nbsp; 1 &lt;= len (s) &lt;= 1000000; <br>Next line, a number N (1 &lt;= N &lt;= 100000), denote that the number of quiries; <br>The next N lines, each line contains a number x (1 &lt;= x &lt;= len (s)).</p>
<h3>Output</h3>
<p>For each x the output F (x);</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>1<br>zaaxbaacbaa<br>11<br>1<br>2<br>3<br>4<br>5<br>6<br>7<br>8<br>9<br>10<br>11<br><br><strong>Output:</strong>
0<br>1<br>2<br>0<br>0<br>1<br>3<br>0<br>0<br>1<br>11</pre>