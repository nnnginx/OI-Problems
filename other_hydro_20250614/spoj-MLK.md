<p><span style="white-space: pre;"> </span>Hareedi and Hanadt live in a village with <strong>N </strong>houses built next to each other along one</p>
<p>straight&nbsp;roadway with equal&nbsp;distances between adjacent houses. Some people own cows</p>
<p>and&nbsp;sell the&nbsp;milk their cows produce, while others do&nbsp;not own cows and may need to buy</p>
<p>milk.</p>
<p>Every morning, Hareedi and Hanadi transport milk around the village&nbsp;such that everyone</p>
<p>buys or sells the exact number of bottles they want. Transporting one bottle of milk from</p>
<p>one house to an adjacent house results in one unit of work. <strong>Fortunately</strong>, the number of</p>
<p>milk bottles needed&nbsp;by people is always equal to the number of milk bottles sold by</p>
<p>cow owners.</p>
<p>&nbsp;</p>
<h3 style="font-size: 1.17em;">Task</h3>
<p>write a program that is given the number of milk bottles that people at each house needs</p>
<p>to buy or sell,&nbsp;represented as an integer, finds the minimum work necessary to transport</p>
<p>the bottles from sellers to buyers.</p>
<p>&nbsp;</p>
<p><strong>Constraints</strong></p>
<p>2 �� <strong>N </strong>�� 1,000,000 &nbsp; &nbsp; The number of houses.</p>
<p>-1000 <strong>��</strong> <strong>B<sub>i</sub>&nbsp;<strong>�� </strong><span style="font-weight: normal;">1000</span></strong><span style="font-size: xx-small; ">&nbsp;&nbsp; &nbsp; &nbsp;<span style="font-size: x-small;">Integer representing the number of bottles to be bought from or</span></span></p>
<p><span style="font-size: xx-small; "><span style="font-size: x-small;">&nbsp;&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;sold to people&nbsp;</span></span><span style="font-size: xx-small;"><span style="font-size: x-small;">at the house at position </span><strong><span style="font-size: x-small;">i.</span></strong></span></p>
<p><strong>Input</strong></p>
<ul>
<li>Line 1 contains the integer <strong>N</strong>, the number of houses.</li>
<li>Each of the next <strong>N</strong>&nbsp;lines contains an integer <strong>B<span style="font-size: xx-small;"><sub>i</sub><span style="font-weight: normal;">.</span>&nbsp;<span style="font-weight: normal;">If <strong>B<span style="font-size: xx-small;"><sub>i</sub></span></strong>&nbsp;&gt; 0 <span style="font-size: x-small;">then people in house </span></span><span style="font-size: x-small;">i</span><span style="font-weight: normal;"><span style="font-size: x-small;"> are cow</span></span></span></strong></li>
</ul>
<p><span style="font-size: xx-small;"><span style="white-space: pre;"><span style="font-size: x-small;"> </span></span><span style="font-size: x-small;">&nbsp;&nbsp;owners and want</span></span><strong><span style="font-weight: normal;"><span style="font-size: x-small;">&nbsp;to sell</span> <strong>B<span style="font-size: xx-small;"><sub>i</sub></span></strong>&nbsp;bottles of milk, If <strong>B<span style="font-size: xx-small;"><sub>i</sub></span></strong>&nbsp;�� 0 then people at house </span>i<span style="font-weight: normal;"> are not cow owners</span></strong></p>
<p><strong><span style="font-weight: normal;"><span style="white-space: pre;"> </span>&nbsp;&nbsp; &nbsp;&nbsp;and want to buy <strong>B<span style="font-size: xx-small;"><sub>i</sub></span></strong>&nbsp;bottles of milk.</span></strong></p>
<p><strong><span style="font-weight: normal;">&nbsp;</span></strong><strong>Output</strong></p>
<ul>
<li>A single line containing a single integer, the minimum work units necessary to</li>
</ul>
<p><span style="white-space: pre;"> </span>&nbsp;&nbsp;transport the bottle&nbsp;of milk.</p>
<ul>
</ul>
<h3>Example</h3>
<pre><strong>Input:</strong>
5</pre>
<pre>5</pre>
<pre>-4</pre>
<pre>1</pre>
<pre>-3</pre>
<pre>1</pre>
<pre><strong>Output:</strong>
9</pre>
<pre>There are 5 houses as shown in the table.</pre>
<pre><span style="white-space: normal; font-size: small;"><table border="1" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td width="72" valign="top">
<p align="center"><strong>Position</strong></p>
</td>
<td width="36" valign="top">
<p align="center"><strong>1</strong></p>
</td>
<td width="36" valign="top">
<p align="center"><strong>2</strong></p>
</td>
<td width="36" valign="top">
<p align="center"><strong>3</strong></p>
</td>
<td width="36" valign="top">
<p align="center"><strong>4</strong></p>
</td>
<td width="36" valign="top">
<p align="center"><strong>5</strong></p>
</td>
</tr>
<tr>
<td width="72" valign="top">
<p align="center"><strong>Bottles</strong></p>
</td>
<td width="36" valign="top">
<p align="center"><strong>5</strong></p>
</td>
<td width="36" valign="top">
<p align="center"><strong>-4</strong></p>
</td>
<td width="36" valign="top">
<p align="center"><strong>1</strong></p>
</td>
<td width="36" valign="top">
<p align="center"><strong>-3</strong></p>
</td>
<td width="36" valign="top">
<p align="center"><strong>1</strong></p>
</td>
</tr>
</tbody>
</table></span></pre>
<pre>4 bottles are transported from house 1 to house 2, 1 bottle from house 1 to</pre>
<pre>house 4, 1 bottle from house 3 to house 4, 1 bottle from house 5 to house 4.</pre>
<pre></pre>
<ul>
<li>
<pre style="color: #000000; font-family: Verdana, Arial, Helvetica, sans-serif; font-size: 10px; margin: 8px;">Number of test-cases is 28.</pre>
</li>
</ul>
<pre></pre>