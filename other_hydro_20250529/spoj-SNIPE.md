<p>Kevin, the Snipe, and her children (apparently Kevin is a girl) were reunited, all thanks to Russell and Mr. Fredricksen! Now the two humans have embarked to their next adventure, towards Poland, but Kevin just noticed her children stole Mr. Fredricksen's cane without him realizing. It must be returned before they go too far away!</p>
<p style="text-align: center;"><img src="./24386/file/H3x9701t.png" alt="" width="445" height="321"></p>
<p>Kevin is not sure where they are now, but knows they went with their flying house somewhere to the northeast, and has narrowed it down to a few points where they might be resting. She will send some of her children to warn them of the missing cane. Each snipe can check multiple places, but since the house should be flying again soon, they can't waste any time and should always move to the north and/or to the east. Additionally, she wants to send the minimum number possible as long as every location on her list is visited.</p>
<p>Your job is to help her determine this number.</p>
<h3>Input</h3>
<p>Input consists of several test cases.&nbsp;</p>
<p>Each test case begins with a single integer <strong>N</strong> (1 ¡Ü <strong>N</strong> ¡Ü 1000), the number of places the house can be.</p>
<p><strong>N</strong> lines follow, each containing two integers, <strong>e<sub>i</sub></strong> and <strong>n<sub>i</sub></strong>, the distance (in miles) to the east and to the north, respectively of the <strong>i</strong><sup>th</sup> place related to Kevin's position. 0 ¡Ü<strong>e<sub>i</sub></strong>, <strong>n<sub>i</sub></strong> ¡Ü= 10000.</p>
<p>Input is terminated by a line containing a single integer zero.</p>
<h3>Output</h3>
<p>For each test case output a single integer: the minimum number of snipes needed to reach every place.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5<br>1 1<br>2 2<br>3 3<br>4 4<br>5 5<br>5<br>1 5<br>2 4<br>3 3<br>4 2<br>5 1<br>5<br>0 1<br>1 1<br>1 2<br>2 2<br>2 3<br>0

<strong>Output:</strong>
1<br>5<br>1
</pre>