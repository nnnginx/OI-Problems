<p><span style="font-size: small;">A fraction tree is an infinite binary tree&nbsp; defined as follows:</span></p>
<p><span style="font-size: small;">1)Every node of tree contains a fraction<br></span></p>
<p><span style="font-size: small;">2)Root of tree contains the fraction 1/1<br></span></p>
<p><span style="font-size: small;">3)Any node with fraction i/j has two children : left child with fraction i/(i+j) and right child with fraction (i+j)/j&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span></p>
<p><span style="font-size: small;">For example , fraction tree upto 3 levels is as shown:</span></p>
<h3 style="text-align: center;"><span style="font-size: small;"><img title="Fraction tree upto 3 levels" src="../../../content/rlewon:NG1FRCTN.png" alt="Fraction tree upto 3 levels" width="313" height="161"></span></h3>
<p><span style="font-size: small;">We number the nodes according to increasing levels ( root is at level 1) and at any same level , nodes are numbered from left to right. So first node holds the fraction 1/1 , second one holds 1/2 , third one holds 2/1 fourth one holds 1/3 and so on.</span></p>
<p><br><span style="font-size: small;">Your task is simple, as always !. Given two numbers a and b , you are to find the product of&nbsp; fractions at all those nodes whose number is between a and b both inclusive.<br></span></p>
<p><span style="font-size: small;">&nbsp;</span></p>
<h3>Input</h3>
<p><span style="font-size: small;">Every line of the input contains two&nbsp; numbers a and b seperated by a space. You are to find the product of all fractions which are at node having number between a and b both inclusive. Input file terminates with a 0 0 which is not to be processed.</span></p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>For each input , print numerator and denominator of the lowest form of the fraction seperated by a /. Output of each case to be done in seperate lines.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>1 1<br>1 2<br>2 4<br>0 0<br><br><strong>Output:</strong><br>1/1<br>1/2<br>1/3<br><br>Constraints : 1&lt;=T &lt;=30000  1&lt;=a&lt;=b&lt;=10^10</pre>
<div id="_mcePaste" style="overflow: hidden; position: absolute; left: -10000px; top: 65px; width: 1px; height: 1px;">1<br>1<br>uQs<br>+<br>Q<br>Q<br>Q<br>Q<br>Q<br>Q<br>Q<br>Q<br>Q<br><br><br><br><br><br><br><br><br>1 <br>2 u<br>e<br>e<br>e<br>e<br>e<br>e<br>%<br>%<br>%<br>%<br>%<br>%<br>2<br>u1<br>e<br>e<br>e<br>e<br>e<br>e<br>%<br>%<br>%<br>%<br>%<br>1 %<br>3<br>u<br>A<br>A<br>A<br>A<br>A<br>A<br><br><br><br><br><br><br>3<br>2<br>uA<br>A<br>A<br>A<br>A<br>A<br><br><br><br><br><br><br>2<br>3<br>uA<br>A<br>A<br>A<br>A<br>A<br><br><br><br><br><br><br>3<br>1<br>uA<br>A<br>A<br>A<br>A<br>A<br><br><br><br><br><br>1 <br>4<br>uA<br>A<br><br><br>4<br>3<br>uA<br>A<br><br><br>3<br>5<br>uA<br>A<br><br><br>5<br>2<br>uA<br>A<br><br><br>2<br>5<br>uA<br>A<br><br><br>5<br>3<br>uA<br>A<br><br><br>3<br>4<br>uA<br>A<br><br><br>4<br>1<br>uA</div>