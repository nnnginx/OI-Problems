<p>N people are lined up in a&nbsp;straight line to enter a concert. Each person&nbsp;in this line knows how many people in front&nbsp;have&nbsp;shorter or same heights. Let's call the sequence&nbsp;representing these numbers S. So in other words, S[i] means that there are S[i] people in front of the ith person who have shorter or same heights than that of&nbsp;person i.&nbsp;</p>
<p>Given the&nbsp;heights of N people and a sequence S, determine the correct&nbsp;order of people lined up. (left is front)&nbsp;&nbsp;&nbsp;</p>
<h3>Input</h3>
<p>The first line of the input is an integer N. (1&lt;=N&lt;=100,000)</p>
<p>The next N lines&nbsp;each consists of one integer&nbsp;H. (1&lt;=H&lt;=2*10^9) These N integers are the heights of people lined up.</p>
<p>Then,&nbsp;sequence S is given in a single&nbsp;line, separated by a space. &nbsp;</p>
<h3>Output</h3>
<p>Determine the correct ordering of people lined up. Total of N lines should be output.&nbsp;The&nbsp;integer on the ith line represents&nbsp;the height of the ith person in the line.&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
12<br>120<br>167<br>163<br>172<br>145<br>134<br>182<br>155<br>167<br>120<br>119<br>156<br>0 1 0 0 3 2 6 7 4 6 9 4<br>
<strong>Output:</strong>
134<br>167<br>120<br>119<br>156<br>120<br>167<br>182<br>155<br>163<br>172<br>145<br>
</pre>