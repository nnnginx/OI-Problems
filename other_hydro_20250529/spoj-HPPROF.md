<p>One day, TA of one of the course at DA-IICT was checking First In-sem exam papers. The exam was of 20 marks. After checking some of the papers, he decided to give marks of those students to his professor but he messed up here. He forgot to put spaces between the marks. So professor got confused.</p>
<p>Since you are his favourite student, help him determine the number of ways in which this marks can be seperated (by spaces) so that they are valid marks.</p>
<p>Marks are valid if they are between 0 to 20 and have no leading zeros. For example, 0, 1, 2, 3 ... 20 are valid but 01, 003, 21, 25 are not valid.</p>
<p><span style="font-size: 1.17em;"><strong>Input</strong></span></p>
<p>Input contains only one line, a string of length less than 20 .</p>
<h3>Output</h3>
<p>Output the number of ways in which you can put spaces and interprete them as a valid marks of students.</p>
<h3>Example</h3>
<pre><strong>Input1 :</strong>
12

<strong>Output1 :</strong>
2<strong><br><br>Input2 :</strong>
111

<strong>Output2 :</strong>
3</pre>
<pre><strong>Input3 :</strong></pre>
<pre>101</pre>
<pre><strong>Output3 :</strong></pre>
<pre>2</pre>
<pre><br><strong>Explaination :</strong></pre>
<pre>In the first case, 12 can be interpreted in two ways,</pre>
<pre>1) 1 2</pre>
<pre>2) 12</pre>
<pre>In the second case, 111 can be interpreted as following ways.</pre>
<pre>1) 1 1 1</pre>
<pre>2) 11 1</pre>
<pre>3) 1 11</pre>
<pre>In the third case,</pre>
<pre>1) 1 0 1</pre>
<pre>2) 10 1</pre>
<pre>Note that 1 01 can not be valid because 01 has leading zeros.</pre>