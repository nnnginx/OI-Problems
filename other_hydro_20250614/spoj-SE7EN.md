<p><span style="font-size: medium;"><span style="font-family: helvetica;">David Mills and William Somerset have teamed up again to catch a criminal. This criminal is a bit different from others, he challenges the detectives by leaving a puzzle at the crime scene which is the clue to his next crime. Both the detectives work hard to crack the puzzle, but the criminal is always one step ahead. For his 7<sup>th</sup> and last crime, he left a problem for the detectives. David wants your help for this one to catch the criminal.</span></span></p>
<p><span style="font-size: medium;"><span style="font-family: helvetica;">The criminal gave you a tree having&nbsp;<strong>n</strong>&nbsp;nodes with&nbsp;<strong>1</strong>&nbsp;as the root. Each node is numbered from 1 to n. Every node has a value represented by the array <strong>A.</strong></span></span></p>
<p><span style="font-size: medium;"><span style="font-family: helvetica;">You are given another array <strong>B.</strong> You have to convert the node values from A to B by performing the minimum number of operations. In one operation you can select any node <strong>i</strong> and add or subtract any value. And the same value will get added to or subtracted from the special node in the subtree of the node <strong>i</strong>.</span></span></p>
<p><span style="font-size: medium;"><span style="font-family: helvetica;">Special node <strong>q </strong>in the subtree of <strong>p </strong>is defined as node such that:</span></span></p>
<p><span style="font-size: medium;"><span style="font-family: helvetica;">(Number of set bits in p) mod 2 = (Number of set bits in q) mod 2</span></span></p>
<p><span style="font-size: medium;"><span style="font-family: helvetica;"> You have to tell the minimum operations to convert node values from A to B and the sum of values added or subtracted in these operations.</span></span></p>
<p><strong><span style="font-size: medium;"><span style="font-family: helvetica;">CONSTRAINTS:</span></span></strong></p>
<p><span style="font-size: medium;"><span style="font-family: helvetica;">1 ¡Ü t ¡Ü 11</span></span></p>
<p><span style="font-size: medium;"><span style="font-family: helvetica;">1 ¡Ü n ¡Ü 10<sup>5</sup></span></span></p>
<p><span style="font-size: medium;"><span style="font-family: helvetica;">1 ¡Ü A[i] ¡Ü 100000</span></span></p>
<p><span style="font-size: medium;"><span style="font-family: helvetica;">1 ¡Ü B[i] ¡Ü 100000</span></span></p>
<h3><span style="font-family: helvetica;"><strong><span style="font-size: medium;"><span style="font-family: helvetica;">INPUT:</span></span></strong></span></h3>
<ol>
<li><span style="font-size: medium;"><span style="font-family: helvetica;">The first line of the input contains a single integer <strong>t</strong>&nbsp;denoting the number of test cases. The description of <strong>t</strong>&nbsp;test cases follows.</span></span></li>
<li><span style="font-size: medium;"><span style="font-family: helvetica;">The first line of each test case contains a single integer <strong>n</strong> denoting the number of nodes.</span></span></li>
<li><span style="font-size: medium;"><span style="font-family: helvetica;">Each of the next&nbsp; n - 1&nbsp;lines contains two integers&nbsp;<em>u<sub>i</sub></em>&nbsp;and&nbsp;<em>v<sub>i </sub></em>(1 ¡Ü <em>u<sub>i</sub></em>, <em>v<sub>i</sub></em> ¡Ü <em>n </em>; <em>u<sub>i</sub></em> ¡Ù <em>v<sub>i</sub></em>) meaning there is an edge between nodes&nbsp;<em>u<sub>i</sub></em>&nbsp;and&nbsp;<em>v<sub>i</sub></em>.</span></span></li>
<li><span style="font-size: medium;"><span style="font-family: helvetica;">Next line has n space-separated integers <strong>A<sub>1</sub>, A<sub>2</sub>, A<sub>3 </sub>,¡­.. A<sub>n</sub></strong> denoting the initial value of nodes. </span></span></li>
<li><span style="font-size: medium;"><span style="font-family: helvetica;">Next line has n space-separated integers <strong>B<sub>1</sub>, B<sub>2</sub>, B<sub>3 </sub>,¡­.. B<sub>n</sub></strong> denoting the final values of nodes.&nbsp;</span></span></li>
</ol>
<h3><span style="font-size: medium;"><span style="font-family: helvetica;">OUTPUT:</span></span></h3>
<p><span style="font-size: medium;"><span style="font-family: helvetica;">Output the minimum number of operations required and the sum of values added or subtracted in these operations.</span></span></p>
<h3><span style="font-size: medium;"><span style="font-family: helvetica;">Example</span></span></h3>
<pre><strong><span style="font-size: small;">Input:</span></strong>
<p>1</p><p>8</p><p>1 3</p><p>3 2</p><p>3 7</p><p>6 2</p><p>4 1</p><p>8 4</p><p>4 5</p><p>9 3 5 6 2 3 8 10</p><p>9 3 3 5 2 1 8 10</p>
<strong><span style="font-size: small;">Output:</span></strong>
<p>3 -2</p></pre>
<p>&nbsp;</p>
<p><strong><span style="text-decoration: underline;"><span style="font-size: small;">Explanation:</span></span></strong></p>
<p><span style="font-size: medium;"><span style="font-family: helvetica;">You can select node 3 with value 5 and subtract 2, it will also get subtracted from the special node 6 in its subtree.</span></span></p>
<p><span style="font-size: medium;"><span style="font-family: helvetica;">Values after 1<sup>st</sup> operation: 9 3 3 6 2 1 8 10</span></span></p>
<p><span style="font-size: medium;"><span style="font-family: helvetica;">Now select node 4 with value 6 and subtract 1, it will also get subtracted from the special node 8 in its subtree.</span></span></p>
<p><span style="font-size: medium;"><span style="font-family: helvetica;">Values after 2<sup>nd</sup> operation: 9 3 3 5 2 1 8 9</span></span></p>
<p><span style="font-size: medium;"><span style="font-family: helvetica;">Now select node 8 and add 1. There is no special node in its subtree.</span></span></p>
<p><span style="font-size: medium;"><span style="font-family: helvetica;">Values after 3<sup>rd</sup> operation: 9 3 3 5 2 1 8 10</span></span></p>
<p><span style="font-size: medium;"><span style="font-family: helvetica;">Sum of values added/subtracted = -2-1+1 = -2</span></span></p>