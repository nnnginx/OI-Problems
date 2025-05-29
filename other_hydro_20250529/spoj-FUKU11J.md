<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/FUKU11J/en/">English</a></td>
<td width="50%"><a href="/problems/FUKU11J/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p></p>
<p style="font-size: medium;"><span style="font-size: small;"><span style="font-size: medium;"><span style="font-family: 'times new roman', times;">Jim is planning to visit one of his best friends in a town in the mountain area. First, he leaves his hometown and goes to the destination town. This is called the go phase. Then, he comes back to his hometown. This is called the return phase. You are expected to write a program to find the minimum total cost of this trip, which is the sum of the costs of the go phase and the return phase.</span></span></span></p>
<p style="font-size: medium;"><span style="font-size: small;"><span style="font-size: medium;"><span style="font-family: 'times new roman', times;">There is a network of towns including these two towns. Every road in this network is one-way, i.e., can only be used towards the specified direction. Each road requires a certain cost to travel.</span></span></span></p>
<p style="font-size: medium;"><span style="font-size: small;"><span style="font-size: medium;"><span style="font-family: 'times new roman', times;">In addition to the cost of roads, it is necessary to pay a specified fee to go through each town on the way. However, since this is the visa fee for the town, it is not necessary to pay the fee on the second or later visit to the same town.</span></span></span></p>
<p style="font-size: medium;"><span style="font-size: small;"><span style="font-size: medium;"><span style="font-family: 'times new roman', times;">The altitude (height) of each town is given. On the go phase, the use of descending roads is inhibited. That is, when going from town&nbsp;<em>a</em>&nbsp;to&nbsp;<em>b</em>, the altitude of&nbsp;<em>a</em>should not be greater than that of&nbsp;<em>b</em>. On the return phase, the use of ascending roads is inhibited in a similar manner. If the altitudes of&nbsp;<em>a</em>&nbsp;and&nbsp;<em>b</em>&nbsp;are equal, the road from&nbsp;<em>a</em>&nbsp;to&nbsp;<em>b</em>&nbsp;can be used on both phases.</span></span></span></p>
<h3><span style="font-size: small;"><span style="font-size: medium;"><span style="font-family: 'times new roman', times;">Input</span></span></span></h3>
<p style="margin-top: 0em; margin-right: 0em; margin-bottom: 1.75em; margin-left: 1px; padding-top: 5px; padding-right: 0px; padding-bottom: 0px; padding-left: 20px; border-top-width: 0px; border-right-width: 0px; border-bottom-width: 0px; border-left-width: 3px; border-style: initial; border-color: initial; outline-width: 0px; outline-style: initial; outline-color: initial; font-size: 16px; vertical-align: baseline; display: block; border-left-style: solid; border-left-color: #dee8ff;"><span style="font-size: small;"><span style="font-size: medium;"><span style="font-family: 'times new roman', times;">The input consists of multiple datasets, each in the following format.</span></span></span></p>
<p style="margin-top: 0em; margin-right: 0em; margin-bottom: 1.75em; margin-left: 1px; padding-top: 5px; padding-right: 0px; padding-bottom: 0px; padding-left: 20px; border-top-width: 0px; border-right-width: 0px; border-bottom-width: 0px; border-left-width: 3px; border-style: initial; border-color: initial; outline-width: 0px; outline-style: initial; outline-color: initial; font-size: 16px; vertical-align: baseline; display: block; border-left-style: solid; border-left-color: #dee8ff;"><em><span style="font-size: small;"><span style="font-size: medium;"><span style="font-family: 'times new roman', times;">n m<br>d<sub>2</sub>&nbsp;e<sub>2</sub><br>d<sub>3</sub>&nbsp;e<sub>3</sub><br>.<br>.<br>.<br>d<sub>n-1</sub> e<sub>n-1</sub><br>a<sub>1</sub>&nbsp;b<sub>1</sub>&nbsp;c<sub>1</sub><br>a<sub>2</sub>&nbsp;b<sub>2</sub>&nbsp;c<sub>2</sub><br>.<br>.<br>.<br>a<sub>m</sub>&nbsp;b<sub>m</sub>&nbsp;c<sub>m</sub></span></span></span></em></p>
<p style="margin-top: 0em; margin-right: 0em; margin-bottom: 1.75em; margin-left: 1px; padding-top: 5px; padding-right: 0px; padding-bottom: 0px; padding-left: 20px; border-top-width: 0px; border-right-width: 0px; border-bottom-width: 0px; border-left-width: 3px; border-style: initial; border-color: initial; outline-width: 0px; outline-style: initial; outline-color: initial; font-size: 16px; vertical-align: baseline; display: block; border-left-style: solid; border-left-color: #dee8ff;"><span style="font-size: small;"><span style="font-size: medium;"><span style="font-family: 'times new roman', times;">Every input item in a dataset is a non-negative integer. Input items in a line are separated by a space.</span></span></span></p>
<p style="margin-top: 0em; margin-right: 0em; margin-bottom: 1.75em; margin-left: 1px; padding-top: 5px; padding-right: 0px; padding-bottom: 0px; padding-left: 20px; border-top-width: 0px; border-right-width: 0px; border-bottom-width: 0px; border-left-width: 3px; border-style: initial; border-color: initial; outline-width: 0px; outline-style: initial; outline-color: initial; font-size: 16px; vertical-align: baseline; display: block; border-left-style: solid; border-left-color: #dee8ff;"><span style="font-size: small;"><span style="font-size: medium;"><span style="font-family: 'times new roman', times;"><em>n</em>&nbsp;is the number of towns in the network.&nbsp;<em>m</em>&nbsp;is the number of (one-way) roads. You can assume the inequalities 2 ≤&nbsp;<em>n</em>&nbsp;≤ 50 and 0 ≤&nbsp;<em>m</em>&nbsp;≤&nbsp;<em>n</em>(<em>n</em>−1) hold. Towns are numbered from 1 to&nbsp;<em>n</em>, inclusive. The town 1 is Jim's hometown, and the town&nbsp;<em>n</em>&nbsp;is the destination town.</span></span></span></p>
<p style="margin-top: 0em; margin-right: 0em; margin-bottom: 1.75em; margin-left: 1px; padding-top: 5px; padding-right: 0px; padding-bottom: 0px; padding-left: 20px; border-top-width: 0px; border-right-width: 0px; border-bottom-width: 0px; border-left-width: 3px; border-style: initial; border-color: initial; outline-width: 0px; outline-style: initial; outline-color: initial; font-size: 16px; vertical-align: baseline; display: block; border-left-style: solid; border-left-color: #dee8ff;"><span style="font-size: small;"><span style="font-size: medium;"><span style="font-family: 'times new roman', times;"><em>d<sub>i</sub></em>&nbsp;is the visa fee of the town&nbsp;<em>i</em>, and&nbsp;<em>e<sub>i</sub></em>&nbsp;is its altitude. You can assume 1 ≤&nbsp;<em>d<sub>i</sub></em>&nbsp;≤ 1000 and 1≤<em>e<sub>i</sub></em>&nbsp;≤ 999 for 2≤<em>i</em>≤<em>n</em>−1. The towns 1 and&nbsp;<em>n</em>&nbsp;do not impose visa fee. The altitude of the town 1 is 0, and that of the town n is 1000. Multiple towns may have the same altitude, but you can assume that there are no more than 10 towns with the same altitude.</span></span></span></p>
<p style="margin-top: 0em; margin-right: 0em; margin-bottom: 1.75em; margin-left: 1px; padding-top: 5px; padding-right: 0px; padding-bottom: 0px; padding-left: 20px; border-top-width: 0px; border-right-width: 0px; border-bottom-width: 0px; border-left-width: 3px; border-style: initial; border-color: initial; outline-width: 0px; outline-style: initial; outline-color: initial; font-size: 16px; vertical-align: baseline; display: block; border-left-style: solid; border-left-color: #dee8ff;"><span style="font-size: small;"><span style="font-size: medium;"><span style="font-family: 'times new roman', times;">The&nbsp;<em>j</em>-th road is from the town&nbsp;<em>a<sub>j</sub></em>&nbsp;to&nbsp;<em>b<sub>j</sub></em>&nbsp;with the cost&nbsp;<em>c<sub>j</sub></em>&nbsp;(1 ≤&nbsp;<em>j</em>&nbsp;≤&nbsp;<em>m</em>). You can assume 1 ≤&nbsp;<em>a<sub>j</sub></em>&nbsp;≤&nbsp;<em>n</em>, 1 ≤&nbsp;<em>b<sub>j</sub></em>&nbsp;≤&nbsp;<em>n</em>, and 1 ≤&nbsp;<em>c<sub>j</sub></em>&nbsp;≤ 1000. You can directly go from&nbsp;<em>a<sub>j</sub></em>&nbsp;to&nbsp;<em>b<sub>j</sub></em>, but not from&nbsp;<em>b<sub>j</sub></em>&nbsp;to&nbsp;<em>a<sub>j</sub></em>&nbsp;unless a road from&nbsp;<em>b<sub>j</sub></em>&nbsp;to&nbsp;<em>a<sub>j</sub></em>&nbsp;is separately given. There are no two roads connecting the same pair of towns towards the same direction, that is, for any&nbsp;<em>i</em>&nbsp;and&nbsp;<em>j</em>&nbsp;such that&nbsp;<em>i</em>&nbsp;≠&nbsp;<em>j</em>,&nbsp;<em>a<sub>i</sub></em>&nbsp;≠&nbsp;<em>a<sub>j</sub></em>&nbsp;or&nbsp;<em>b<sub>i</sub></em>&nbsp;≠&nbsp;<em>b<sub>j</sub></em>. There are no roads connecting a town to itself, that is, for any&nbsp;<em>j</em>,&nbsp;<em>a<sub>j</sub></em>≠&nbsp;<em>b<sub>j</sub></em>.</span></span></span></p>
<p style="margin-top: 0em; margin-right: 0em; margin-bottom: 1.75em; margin-left: 1px; padding-top: 5px; padding-right: 0px; padding-bottom: 0px; padding-left: 20px; border-top-width: 0px; border-right-width: 0px; border-bottom-width: 0px; border-left-width: 3px; border-style: initial; border-color: initial; outline-width: 0px; outline-style: initial; outline-color: initial; font-size: 16px; vertical-align: baseline; display: block; border-left-style: solid; border-left-color: #dee8ff;"><span style="font-size: small;"><span style="font-size: medium;"><span style="font-family: 'times new roman', times;">The last dataset is followed by a line containing two zeros (separated by a space).</span></span></span></p>
<h3><span style="font-size: small;"><span style="font-size: medium;"><span style="font-family: 'times new roman', times;">Output</span></span></span></h3>
<p><span style="font-size: small;"><span style="font-size: medium;"><span style="font-family: 'times new roman', times;"> For each dataset in the input, a line containing the minimum total cost, including the visa fees, of the trip should be output. If such a trip is not possible, output “-1”.</span></span></span></p>
<h3><span style="font-size: small;"><span style="font-size: medium;"><span style="font-family: 'times new roman', times;">Example</span></span></span></h3>
<pre><span style="font-size: small;"><span style="font-size: medium;"><span style="font-family: 'times new roman', times;"><strong>Input:</strong>
3 6
3 1
1 2 1
2 3 1
3 2 1
2 1 1
1 3 4
3 1 4
3 6
5 1
1 2 1
2 3 1
3 2 1
2 1 1
1 3 4
3 1 4
4 5
3 1
3 1
1 2 5
2 3 5
3 4 5
4 2 5
3 1 5
2 1
2 1 1
0 0

<strong>Output:</strong>
7
8
36
-1</span></span></span>
</pre>
<p> </p>