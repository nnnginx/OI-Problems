<p>With the coming release of Marcohard Balconies 100 operating system, people are more and more interested in its new UI (User Interface), code-named ¡°Subway¡±.</p>
<p>This UI presents your desktop as a grid that is divided into <strong>N</strong> rows and <strong>M</strong> columns (so you have <strong>N</strong> * <strong>M</strong> cells). In each cell, you can place one icon of an application of a certain type. Your applications can be of one of <strong>K</strong> types, numbered 1 through K. You¡¯re an expert in this field, so it is assumed that there is an unlimited number of applications of each type.</p>
<p>Any placement is called an icon formation. Some of the icon formations are beautiful. An icon formation is called beautiful if and only if no pair of rows are similar. Two rows are similar if and only if for each <em>X</em> that 1 &lt;= <em>X</em> &lt;= <strong>K</strong>, they contain exactly the same number of applications of type <em>X</em>.</p>
<p>Given <strong>N</strong>, <strong>M</strong>, and <strong>K</strong>, you should solve for the number of different icon formations that are beautiful, modulo 10<sup>9</sup>+7. Two formations are different if and only if there is a cell where the type of application in one formation is not the same as the type in another formation.</p>
<p>You may assume that 1 &lt;= <b>N</b>, <b>M</b>, <b>K</b> &lt;= 50.</p>
<h3>Input</h3>
<p>There are several test cases. For each test case there are 3 integers, named <strong>N</strong>, <strong>M</strong>, <strong>K</strong>, in a single line. Please process until EOF (End Of File).</p>
<h3>Output</h3>
<p>For each test case, please print a single line with a integer, the corresponding answer to this case.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2 2 2
5 3 2
3 5 7

<strong>Output:</strong>
10
0
894953467
</pre>