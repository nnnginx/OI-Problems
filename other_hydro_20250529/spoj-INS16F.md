<p>Baratheon is one of the oldest houses in the Land of Seven Kingdoms. There have been many kings and their many heirs. The hierarchy is represented as a tree where each character is a node with initial value as the <strong>Varys_Value</strong> given by Lord Varys. You are the analyser appointed to the current King to give insights about a character.</p>

<p>There are <strong>Q</strong> commands given by the King which can be any of the following type:<br>1. Multiply the <strong>Varys_Value</strong> of all the characters in path from <strong>u</strong> to <strong>v</strong> by a given number <strong>P.</strong><br>2. For a given character <strong>X</strong>, find the number of <strong>ordered pairs (i,j) </strong>such that <strong>LCM(i,j)</strong> is equal to current value at node <strong>X</strong>. (Insight)</p>
<p>For commands of second type, print the number of such pairs (modulo <strong>1000000007</strong>).</p>

<h3>Input</h3>
<p>First line contains 2 space separated integers <strong>N</strong> and <strong>Q</strong> indicating the number of total characters and number of queries you need to answer.</p>

<p>In the next <strong>N-1</strong> lines, each line contains 2 integers <strong>u</strong>, <strong>v</strong> which indicates a relationship between character <strong>u</strong> and character <strong>v</strong>.</p>

<p>Next line contains <strong>N</strong> space separated integer <strong>V<sub>1</sub>, V<sub>2</sub>, V<sub>3</sub>, ...... V<sub>N</sub></strong> where <strong>V<sub>i</sub></strong> indicates the Varys_Value of <strong>i<sup>th</sup></strong> character.</p>

<p>Following <strong>Q</strong> lines contains the queries to be answered.<br>Types of Queries:</p>
<p><strong>1 u v P</strong> - Query of first type</p>
<p><strong>2 X </strong>- Query of second type</p>

<h3>Output</h3>
<p>For each query of second type, print the answer to the query in a new line.</p>

<h3>Constraints</h3>
<p>1 ¡Ü N ¡Ü 100000<br>
1 ¡Ü Q ¡Ü 100000<br>
1 ¡Ü u, v ¡Ü N<br>
1 ¡Ü P ¡Ü 100<br>
1 ¡Ü V<sub>i</sub> ¡Ü 100000</p>

<h3>Example</h3>
<pre><b>Sample Input:</b>
6 6 
1 2
4 6
1 3
5 1
4 5
7 8 4 8 1 2
1 2 1 14
2 4
1 6 5 10
2 5
1 6 4 10
2 1

<b>Sample Output:</b>
7
9
15</pre>