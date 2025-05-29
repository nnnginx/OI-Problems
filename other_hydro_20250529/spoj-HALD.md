<p>Hiccup is the king of Viking village of Berk which is full of dragons. Like every year, Dragon War contest is going to be organized in Berk in which dragons fight till certain time limit and winning group of dragons are embraced as&nbsp; lucky dragon group for the village. Each dragon is characterized by its unique power level Pi. There are N dragons in the village with each dragon having a power level in the range [1,N]. No two dragons have the same power level. Hiccup does not want Dragons to fight so he comes up with a new strategy to select the required group of Dragons. He tells the villagers the he had a dream last night in which his father told him that a group of dragons will be lucky for the village if following two conditions are satisfied:<br>1) There are at least two dragons in the group.<br>2) Difference in the power level of any two dragons in the group is at least two.<br><br>Hiccup is going to choose any random lucky group of dragons to avoid the Dragon War but first he wants to know how many such groups are possible.</p>
<h3>Input</h3>
<p>First line of input contains T i.e. number of test cases. Next T lines contains an integer N denoting number of dragons in the village followed by an integer M.</p>
<h3>Output</h3>
<p>Print (number of lucky dragon groups possible) % M for each N</p>
<h3>Constraints:</h3>
<p>1 &lt;= T &lt;= 100000<br>1 &lt;= N &lt;= 10^18<br>1 &lt;= M &lt;= 10^18</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2<br>1 3<br>3 2

<strong>Output:</strong>
0<br>1<br><br></pre>
<h3>Explanation of sample input, n = 3 and m = 2:</h3>
<pre>There will be 3 dragons with power level 1,2,3 respectively.<br>Only 1 group can be chosen i.e {1,3}. So answer is (1 % 2) = 1 <br></pre>