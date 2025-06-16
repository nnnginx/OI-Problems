<div>
<p><span style="font-size: 12.000000pt; font-family: 'LiberationSerif';">Based on the latest intelligence reports, Chief Arnook of the northern tribe has become suspicious of the warrior nations that dwell south of the border. The chief has ordered his warriors to protect the southern border which runs parallel to the 54<sup>o</sup> latitude line and stretches between the longitudes of 1<sup>o</sup> to 1000,000,000<sup>o</sup>, inclusive. </span></p>
<p><span style="font-size: 12.000000pt; font-family: 'LiberationSerif';">Each warrior is assigned the task of protecting a segment of the border defined to lie between longitudes ¡°a¡± and ¡°b¡±, inclusive. No two warriors are assigned to protect the exact same segment. Bound by loyalty to his chief, a warrior will inform the chief upon his arrival at his appointed post and will never leave once he arrives.&nbsp;</span></p>
<div>
<div>
<div>
<div>
<p><span style="font-size: 12.000000pt; font-family: 'LiberationSerif';">Your task is to write a program that performs the following two operations <span style="font-size: 12.000000pt; font-family: 'LiberationSerif';">to help Chief Arnook track the status of his border protection. &nbsp; &nbsp;</span></span></p>
</div>
</div>
</div>
<div>
<div>
<p>&nbsp;</p>
<p><span style="font-size: 12.000000pt; font-family: 'LiberationSerif';">+ a b</span></p>
<p><span style="font-size: 12.000000pt; font-family: 'LiberationSerif';">a warrior assumes his position and protects the segment between longitudes ¡°a¡± and ¡°b¡±, inclusive.</span></p>
<p>&nbsp;</p>
<p><span style="font-size: 12.000000pt; font-family: 'LiberationSerif';">? c d &nbsp; &nbsp; &nbsp; &nbsp;</span></p>
<div>
<div>
<div>
<p><span style="font-size: 12.000000pt; font-family: 'LiberationSerif';">computes the number of warriors who completely protect the segment between longitudes ¡°c¡± and ¡°d¡±, inclusive. The segment between the longitudes ¡°c¡± and ¡°d¡±, inclusive, is said to be completely protected by a warrior X if and only if warrior X protects a segment between </span></p>
</div>
</div>
<div>
<div>
<div>
<p><span style="font-size: 12.000000pt; font-family: 'LiberationSerif';">¡°a¡± and ¡°b¡±, inclusive, and a ¡Ü c ¡Ü&nbsp;d ¡Ü b.<br> </span></p>
</div>
</div>
</div>
</div>
<p><span style="font-family: LiberationSerif;"><br></span><span style="font-size: 12.000000pt; font-family: 'LiberationSerif';">&nbsp;</span></p>
</div>
<div>
<h3><strong>Input</strong></h3>
</div>
</div>
</div>
</div>
<p><span style="font-size: 12.000000pt; font-family: 'LiberationSerif';">The input starts with an integer N (1 ¡Ü&nbsp;N ¡Ü&nbsp;500000), on a line by itself, that indicates the number of operations. Each of the following N lines contains one operation. The description of an operation consists of a character ¡°+¡± or ¡°?¡± followed by two integers on a line by itself. The entries on a line are separated by single blank spaces.&nbsp;</span></p>
<p><span style="font-size: 12.000000pt; font-family: 'LiberationSerif';"><br></span></p>
<h3>Output</h3>
<p><span style="font-size: 12.000000pt; font-family: 'LiberationSerif';">There is one output line for each input line that starts with the operation ¡°?¡±. The output consists of a single integer that represents the number of warriors who completely protect the corresponding segment at the time.&nbsp;</span></p>
<p><span style="font-size: 12.000000pt; font-family: 'LiberationSerif';"><span style="font-size: 12.000000pt; font-family: 'LiberationSerif';">There is no output for input lines that start with the character ¡°+¡±. &nbsp; &nbsp;</span></span></p>
<h3>Example</h3>
<pre><strong>Input:</strong>
9
+ 5 10
+ 7 20
+ 3 15
? 9 12
+ 10 20
? 8 9
+ 6 30
? 8 9
? 9 12

<strong>Output:</strong>
2
3
4
3</pre>