<p>Mirza is a fresher of IUT(International University Of Technology). Today is his fresher's reception day. His senior brother's arranged an amazing function on that occasion. N best music bands of the country came to perform in his campuss. As per sunset rules, they had to shorten the timespan of the program. So, all the N bands are performing in different auditoriams at the same time. After each song of each band there is a break , when if you wish you can go from one auditorium to other, but not inbetween the songs. And also you want to enjoy the most.</p>
<p>Now, there is a fun value for each song played by each band. When you are listening to a band for the first time, you'll enjoy the most. Then if you hear a song for the second time you'll enjoy less. The value will decrease by times.</p>
<p>More formal: for a specific band i, There is two fun coefficients a<sub>i</sub> and b<sub>i</sub> . While listening a song of a perticular band for the k-th time, Mirza gains a enjoyment value of&nbsp; f(i, k) = a<sub>i</sub> − (k − 1)<sup>2</sup>&nbsp;* b<sub>i</sub> . If f(i, k) is non-positive, listening a song to that band is no longer enjoyable. Note:[If you enjoyed 1st song of a band then go to other auditorum and miss the second song of this band and come back again for the 3rd song, the 3rd song of this band will count as 2nd for you as you are listening them for the 2nd time]</p>
<p>Given the maximum time Mirza can spent in the auditoriums, can you tell the maximum enjoyment value of Mirza.</p>
<h3>Input</h3>
<p>The first line contains the integer N, where N is the number of band came to perform (0 &lt; N ≤ 100). The following N lines contain the integers a<sub>i</sub> , b<sub>i</sub> and t<sub>i</sub> where a<sub>i</sub> and b<sub>i</sub> are the fun coefficients as specified above and t<sub>i</sub> is the length of each song played by the i-th band (0 ≤ a<sub>i</sub> ≤ 2500; 0 ≤ b<sub>i</sub> ≤ 2500; 0 &lt; t<sub>i</sub> ≤ 50000). The next line contains a positive integer Q denoting the number of Query (0 ≤ Q ≤ 1000). Each of the following Q lines contains an integral time T&nbsp;that Mirza spends in auditorium his (0 ≤ T ≤ 50000).</p>
<h3>Output</h3>
<p>For each query, Print an integer denotion the maximim enjoyment value Mirza can get.</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre>2 </pre>
<pre>5 0 5 </pre>
<pre>7 0 7 </pre>
<pre>4 </pre>
<pre>88 </pre>
<pre>5 </pre>
<pre>6 </pre>
<pre>7

<strong>Output:</strong></pre>
<pre>88 </pre>
<pre>5 </pre>
<pre>5 </pre>
<pre>7</pre>
<pre><pre><strong><br></strong></pre>
<pre><strong>Input:</strong></pre>
<pre>1 </pre>
<pre>100 3 2 </pre>
<pre>5 </pre>
<pre>2 </pre>
<pre>3 </pre>
<pre>4 </pre>
<pre>5 </pre>
<pre>100</pre>
<pre><strong>Output:</strong></pre>
<pre>100 </pre>
<pre>100 </pre>
<pre>197 </pre>
<pre>197 </pre>
<pre>435</pre>
</pre>