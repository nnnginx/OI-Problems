<p>Gauthami has to get dressed for a date. She is going to meet Prasanna in the poshest restaurant in the country of Thuvax. <br>Prasanna arrives early and sees the outfit she has picked. &nbsp;<br>While waiting outside, Prasanna being a restless nerd calculates the number of ways she can get dressed. <br>&nbsp;<br>The complete outfit she picks is represented as a string of digits.&nbsp;The digits represent the following details about the apparel: <br>(apparel = clothing or accessories or any other part of the outfit) <br>&nbsp;<br>1 - a 2 piece apparel where first piece has to be worn before the other. It is followed by the description of the two pieces in order.<br>&nbsp;<br>2 - a 2 piece apparel which can be worn in any order, and it is not necessary to complete one apparel before starting another one. It is followed by the description of the two pieces in order.<br>&nbsp;<br>0 - a single piece of apparel which can be put on directly. <br>&nbsp;<br>Help Prasanna calculate the number of ways in which Gautami can get dressed. Since Prasanna does not want to make Gauthami bored by telling her a huge number, he wants to tell her the number of ways modulo 1000000007.<br>&nbsp;<br>For example, consider an outfit comprising of a shirt, a skirt into which the shirt has to be tucked in and &nbsp;<br>a neck cloth worn over the shirt. <br>It will be represented as 10200 and the number of ways she can get dressed is 2(She has to wear the shirt first after which she can wear either the skirt after the neck cloth or neck cloth after the skirt).</p>
<p><strong>Input</strong></p>
<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">First line is a positive integer T (T&lt;=100) representing the number of testcases&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">It is followed by T lines, each containing a string S of digits (each digit will be one of 0,1,2) describing the outfit, 1&lt;=|S|&lt;=100,000</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The complete outfit comprises of a single item.</div>
<p>
</p><p>First line is a positive integer T (T&lt;=100) representing the number of testcases&nbsp;</p>
<p>It is followed by T lines, each containing a string S of digits (each digit will be one of 0,1,2) describing the outfit, 1&lt;=|S|&lt;=100,000</p>
<p>The complete outfit comprises of a single item.</p>
<p></p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>Output for each test case should consist of one line representing the number of ways in which Gauthami can get dressed modulo 1000000007.</p>
<p><strong>Example</strong></p>
<pre><strong>Input:</strong>
3 <br>10200 <br>0 <br>1102000

<strong>Output:</strong>
2 <br>1 <br>2<span style="white-space: normal;">
</span></pre>