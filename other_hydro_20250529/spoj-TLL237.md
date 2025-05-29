<pre style="font-family: 'Bitstream Vera Sans Mono', Monaco, Consolas, 'Courier New', monospace; font-size: 12px; line-height: 15.600000381469727px; margin-top: 0em;"><span style="padding-top: 0.2em; padding-bottom: 0.1em;">jhon is compulsive saver, he keeps and amount "n" of piggy banks locked in his room.
</span>
<span style="padding-top: 0.2em; padding-bottom: 0.1em;">He has a list which he wrote with a sequence of 1's and 2's that indicate the way that Jhon will 
deposit his money on the piggy banks. Every time Jhon gets a penny he rushes to his room and 
picks the 2 piggy banks who have the less amount of money, then he looks at the next number 
on the sequence. If that number is one (1) he deposits the penny on the piggy bank with the lesser 
amount of money. If that number is two (2) he deposits the penny on the next piggy bank with 
the lesser amount of money.
</span>
<span style="padding-top: 0.2em; padding-bottom: 0.1em;">Your task is to write a program to help Jhon to determine what is the amount in the 2 piggy 
banks with less money once the sequence is over
</span><span style="padding-top: 0.2em; padding-bottom: 0.1em;">
if more than two have the lowest amount of money choose those with lowest indexes.</span></pre>
<pre style="font-family: 'Bitstream Vera Sans Mono', Monaco, Consolas, 'Courier New', monospace; font-size: 12px; line-height: 15.600000381469727px; margin-top: 0em;">you can assume that n &lt;= s</pre>
<h3>Input</h3>
<pre style="font-family: 'Bitstream Vera Sans Mono', Monaco, Consolas, 'Courier New', monospace; font-size: 12px; line-height: 15.600000381469727px; margin-top: 0em;"><span style="padding-top: 0.2em; padding-bottom: 0.1em;">the input is a unique date set
</span>
<span style="padding-top: 0.2em; padding-bottom: 0.1em;">n is the number of piggy banks, 2 &lt;= n &lt;= 10^5
s is the sequence with 1's and 2's, 1 &lt;= size(s)  &lt;= 10^5</span><span style="padding-top: 0.2em; padding-bottom: 0.1em;"><br></span></pre>
<h3>Output</h3>
<pre style="font-family: 'Bitstream Vera Sans Mono', Monaco, Consolas, 'Courier New', monospace; font-size: 12px; margin-top: 0em; line-height: 15.600000381469727px;"><span style="padding-top: 0.2em; padding-bottom: 0.1em;">a line containing what is the amount in the 2 piggy banks with less money once the sequence is over, 
sorted from lowest to highest.</span></pre>
<p>Example</p>
<pre><strong>Input:</strong>
3</pre>
<pre>111112

<strong>Output:</strong>
1 2</pre>