<p align="justify">
Your task is to calculate the result of the hashing process in a table of 101 elements, containing keys that are strings of length at most 15 letters (ASCII codes '<i>A</i>',...,'<i>z</i>'). 
Implement the following operations:
</p><div align="left">
<ul>
<li>find the index of the element defined by the key (ignore, if no such element),
</li><li>insert a new key into the table (ignore insertion of the key that already exists),
</li><li>delete a key from the table (without moving the others),
by marking the position in table as <i>empty</i> (ignore non-existing keys in the table)
</li></ul></div>
<p>When performing find, insert and delete operations define the following function: <br>
<i>integer Hash(string key)</i>,<br>which for a string <i>key</i>=<i>a</i><sub>1</sub>...<i>a<sub>n</sub></i> returns the value:<br>
<i>Hash</i>(<i>key</i>)=<i>h</i>(<i>key</i>) mod 101, where
<br><i>h</i>(<i>key</i>)=19 *(ASCII(<i>a</i><sub>1</sub>)*1+...+ASCII(<i>a<sub>n</sub></i>)*<i>n</i>).<br>Resolve collisions using the open addressing method, i.e. try to insert the key into the table at the first free position: (<i>Hash</i>(<i>key</i>)+<i>j</i><sup>2</sup>+23*<i>j</i>) mod 101, for <i>j</i>=1,...,19.
After examining of at least 20 table entries, we assume that the insert operation cannot be performed.
</p>
<h3>Input</h3>
<p align="justify">
<br><i>t</i> [the number of test cases &lt;= 100]
<br><i>n</i><sub>1</sub> [the number of operations (one per line)[&lt;= 1000] 
<br>ADD:string
<br>[or]
<br>DEL:string
[other test cases, without empty lines betwee series]
</p>
<h3>Output</h3>
<p align="justify">
For every test case you have to create a new table, insert or delete keys, and write to the output:
<br>
the number of keys in the table [first line]
<br>index:key [sorted by indices]
</p>
<h3>Example</h3>
<pre>Input:
1
11
ADD:marsz
ADD:marsz
ADD:Dabrowski
ADD:z
ADD:ziemii
ADD:wloskiej
ADD:do
ADD:Polski
DEL:od
DEL:do
DEL:wloskiej
<!--
8
ADD:my
ADD:favourite
ADD:online
ADD:judge
ADD:sphere!
DEL:judge
DEL:my
DEL:my-->

Output:
5
34:Dabrowski
46:Polski
63:marsz
76:ziemii
96:z
<!--3
15:sphere!
37:favourite
70:online-->
</pre>