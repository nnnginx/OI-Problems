<p>Every time someone is preparing to be interviewed, there is someone  preparing the interview. While a good guy is preparing for the interview  described in <a title="ILKQUERY" href="../ILKQUERY/">http://www.spoj.com/problems/ILKQUERY/</a>&nbsp; your boss gives you the job of preparing the  input/output for a new task.<br><br>But as always, your boss changes his mind so quickly... He will give you an array of integers, but sometime, he will say you that the element at index <strong>r </strong>of the original array must toggle his state between active (1) and inactive (0).<br>Initially all elements start as active elements. <br>Toggle the state of an element means to change it to active (1) if it was inactive, and change it to inactive (0) if it was active.<br><br>Mixed with the toggle operations, he also will give you several queries, represented with three integers, <strong>i l k</strong> meaning he wants to know how many active elements of value <strong>k</strong> exist between indexes<strong> i</strong> and <strong>l</strong> (both inclusive)</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>Input consists of one test case.</p>
<p>The first line contains two integers, <strong>N</strong> ( 1 ¡Ü&nbsp; N&nbsp; ¡Ü&nbsp; 10<sup>5</sup>) and <strong>Q</strong> (1 ¡Ü Q&nbsp; ¡Ü 10<sup>5</sup>).</p>
<p>The next line contains <strong>N</strong>&nbsp; integers <strong>a<sub>i</sub></strong> ( -10<sup>9</sup>&nbsp; ¡Ü a<sub>i</sub> ¡Ü 10<sup>9</sup>).</p>
<p>Then <strong>Q</strong> lines follow. Each of them starts with an integer <strong>q</strong> which can be 0 or 1. If it's 0, then three integers <strong>i l k</strong> follow (0 ¡Ü i &lt; N ; i ¡Ü l &lt; N ; -10<sup>9</sup> ¡Ü k ¡Ü 10<sup>9</sup>). If it's 1, then an integer <strong>r</strong> follows, meaning you have to toggle the state of the element at index <strong>r</strong>. (0 ¡Ü r &lt; N).</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>For each query starting with 0 (in the same order as the input) output a  single line with the answer to that query. That is, output the amount  of active elements of value <strong>k</strong> between the indexes <strong>i</strong> and <strong>l</strong> (both  inclusive).</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
10 5<br>2 2 3 2 1 5 4 2 6 3<br>0 0 7 2<br>1 3<br>0 0 7 2<br>1 6<br>0 2 7 4<br><strong>Output:</strong>
4<br>3<br>0</pre>