<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/TWINSNOW/en/">English</a></td>
<td width="50%"><a href="/problems/TWINSNOW/vn/">Tiếng Việt</a></td> 
</tr></tbody></table>

<p>
You may have heard that no two snowflakes are alike. Your task is to write a program to determine whether this is really true. Your program will read information about a collection of snowflakes, and search for a pair that may be identical. Each snowflake has six arms. For each snowflake, your program will be provided with a measurement of the length of each of the six arms. Any pair of snowflakes which have the same lengths of corresponding arms should be agged by your program as possibly identical.
</p>

<center><img src="./24798/file/yyCkdBoY.png"></center>

<h3>Input</h3>
<p>
- The first line of input will contain a single integer n; the number of snowflakes to follow.
<br>- This will be followed by n lines, each describing a snowflake. Each snowflake will be described by a line containing six integers (each integer is at least 0 and less than 10000000), the lengths of the arms of the snowflake. The lengths of the arms will be given in order around the snowflake (either clockwise or counterclockwise), but they may begin with any of the six arms. For example, the same snowflake could be described as 1 2 3 4 5 6 or 4 3 2 1 6 5.
</p>

<h3>Output</h3>
<p>
If all of the snowflakes are distinct, your program should print the message:
</p>
<pre><b>No two snowflakes are alike.</b></pre>
<p>
If there is a pair of possibly identical snowflakes, your program should print the message:
</p>
<pre><b>Twin snowflakes found.</b></pre>

<h3>Sample</h3>

<pre><b>Input:</b>
2
1 2 3 4 5 6
3 4 5 6 1 2

<b>Output:</b>
Twin snowflakes found.
</pre>

<h3>Limitations</h3>
<p>- 0 &lt; n ≤ 10<sup>5</sup>.
</p>