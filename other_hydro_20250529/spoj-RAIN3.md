<p>Doctor Jones is a famous archeologist. He did some research on the Tiribaki Islands recently. His most famous discovery was the Meteoronome - a machine with a yellow button used by the Tiribakian highest priest to predict the weather. The Meteoronome had been set up by the gods at the Beginning of Time. Tiribakians pressed the button every day. As a result, the Meteoronome produced a number - the expected rainfall in millimetres for the next day. More precisely, after <i>i</i> button hits (counted since the Beginning of Time) Meteoronome gives the expected rainfall for the day <i>i</i> since the Beginning of Time. </p>

<p>Unfortunately, the Meteoronome has not been used for several thousands of years and nobody knows how many steps should be performed to reach the current date. Researchers have spent a lot of effort to find out how the Meteoronome works. A mathematical model has been proposed: The Meteoronome is initialized by a pair of integers, s[0] and t[0]. For the <i>i</i>-th step, the Meteoronome computes the values </p>
<pre>s[i] = (78901 + 31*s[i-1]) mod  699037
t[i] = (23456 + 64*t[i-1]) mod 2097151
</pre>
<p>The output of the i-th step is the number</p>
<pre>a[i]=(s[i] mod 100 + 1) * (t[i] mod 100 + 1)
</pre>
<p>Doctor Jones's friend, Ms. Linda Watson, is now planning a holiday on Tiribaki Islands. She would like to stay there as long as possible but she hates the rain. She can stand no more than M millimetres of rainfall during her entire stay on Tiribaki. </p>

<p>Doctor Jones wants to help his friend and to compute the longest period which she can safely stay on Tiribaki. He simulated <i>N</i> steps of the Meteoronome. This way, he obtained a sequence of numbers a[1],a[2],...,a[N] which represent predictions for <i>N</i> subsequent days. Now he wants to find the largest <i>K</i> such that for each period of at most <i>K</i> subsequent days from day <i>i</i> to day <i>j</i> the sum of the predictions a[i]+a[i+1]+...+a[j] is less than or equal to <i>M</i>. Linda can be sure that if she stays on Tiribaki for at most <i>K</i> days, she can endure the rain (provided that <i>N</i> is large enough). 

</p><h3>Input specification</h3>
<p>The input file consists of several blocks of data. The first line of the input file contains the number of blocks. Each block contains four integers delimited by whitespace: s[0], t[0] - the initial values for the Meteoronome, <i>N</i> (1&lt;= <i>N</i> &lt;=1500000)- the length of the sequence and <i>M</i> - the maximum sum of a subsequence. All the input data fits into 32-bit signed integer.</p>

<h3>Output specification</h3>
<p>The output file contains one line for each block of input data. In this line there is a single integer <i>K</i> as specified above. </p>

<h3>Example</h3>
<pre><b>Input file:</b>
1
123456 123456 10 10000

<b>Output file:</b>
2
</pre>
<p>Note, that the sequence produced by Meteoronome for this input file is 4664,1248,267,4900,837,4048,990,6935,1155,490. No subsequence of length 2 has sum greater than 10000 and there are subsequences of length 3 with greater sum.</p>