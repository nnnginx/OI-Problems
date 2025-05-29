<p>Kumar was very excited for his Valentine's day but at the same time he was afraid about the demands of his date.</p>
<p><br>All was going good, but at last they ordered wine, waiter offered x and y unit glasses, here she got him, she said "I will drink only z unit, it's a crime not to eat a rare steak without a good glass of red wine".<br>Now to get the z unit out of x and y unit of glasses, Kumar starts shuffling wine from one glass to another, as it will impress her, he had to do it quick, he does't want to get embarrassed by calling for other glasses, or making other excuses.</p>
<p>Guess how he managed to serve the wine.</p>
<h3>Input</h3>
<p>First line contains x and y. Next line contains q number of possible values of z his date can demand.<br>Next q line contains values of z.</p>
<h3>Output</h3>
<p>For each z, output the minimum step required to serve z unit of wine with the available glasses even if he needs to waste some or output "Damn!!" if he can't serve.</p>
<p>Format for output<br>Case &lt;ith query&gt;: &lt;output&gt;</p>
<h3>Constraints</h3>
<p>0 &lt;= x,y &lt;= 1000 (Yes, 0 mean waiter doesn't even serve the glasses).<br>0 &lt;= z &lt;= 2000 (0 means, she doesn't wanted to drink at all, ordering wine was just the Kumar's choice).</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2 3<br>6<br>0<br>1<br>2<br>3<br>4<br>6

<strong>Output:</strong>
Case 1: 0<br>Case 2: 2<br>Case 3: 1<br>Case 4: 1<br>Case 5: 3<br>Case 6: Damn!!<br><br><strong>Explanation:<br><br></strong>Case 2: (0,3) -&gt; (2,1)<br>Case 5: (2,0) -&gt; (0,2) -&gt; (2,2)<br>Case 6: He can't serve.</pre>