<p>There are N classes in a school, each with M students. There is going to be a race&nbsp;of 100m dash, and a representative from&nbsp;each class&nbsp;will be chosen to&nbsp;participate in this race. You were assigned a task to choose these representatives. Since you did not want the race to be one sided, you wanted to choose the representatives such that the difference between the&nbsp;ability of&nbsp;the best&nbsp;representative and the&nbsp;worst representative&nbsp;is minimal.</p>
<p>For example, if N = 3 and M = 4, and each class has&nbsp;students with following abilities:</p>
<p>Class 1: {12,16,67,43}</p>
<p>Class 2: {7,17,68,48}</p>
<p>Class 3: {14,15,77,54}</p>
<p>it is best to choose the student with ability 16 from Class 1, 17 from Class 2, and 15 from Class 3. Thus, the difference in this case would be 17-15 = 2.</p>
<p>Your task is to calculate the minimal possible difference you can achieve by choosing a representative from each class.</p>
<h3>Input</h3>
<p>The first line of the input consists of two integers, N and M. (1&lt;=N&lt;=1000, 1&lt;=M&lt;=1000).</p>
<p>The next N lines will have M integers. The jth element of ith line is the ability of the jth student in ith class. The number is between 0 and 10^9, inclusive.</p>
<h3>Output</h3>
<p>Output the minimal difference one can achieve by choosing the representative from each class.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3 4<br>12 16 67 43<br>7 17 68 48<br>14 15 77 54<br><br>
<strong>Output:</strong>
2</pre>
<pre><strong></strong></pre>
<pre><strong>Input:</strong><br>4 3<br>10 20 30<br>40 50 60<br>70 80 90<br>100 110 120</pre>
<pre><br><br><br><br><strong>Output:</strong><br>70<br><br><br></pre>