<p> The niceness of a string s (s comprises of a-z, A-Z and space characters only) is calculated using steps given below.</p>
<ol>
  <li>First seperate out the string into continous non zero length string without space. eg. Let us take s = "now do it now". You can break this into four small strings as "now", "do", "it" and "now". Call the set of these small strings to be G.</li>
  <li>Now reverse all the strings in G. eg. "won", "od", "ti", "won".</li>
  <li>Finally you calculate number of distinct strings in you set. in this case answer is 3. as "won", "od" and "ti" are set of distinct strings. Note that "won" comes twice but counted only once.</li>
</ol>
<p>So you have to find niceness value of a string s.</p>
<p>Note that given string s can contain more than one continous spaces. eg. "now do it now ". Niceness value of this is also same as above given example.</p>

<h3>Input</h3>
<p>T: number of test cases. (T &lt;= 100)</p>
<p>for next T lines, every line contains one string s (1 &lt;= |s| &lt;= 10<sup>4</sup>)</p>

<h3>Output</h3>
<p>For every test case, output niceness value of given string s.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
4
now do it now
now      do it now
I am  good boy
am am

<strong>Output:</strong>
3
3
4
1</pre>