<p>King of Boxes Robert wants to test Samvel.&nbsp; He has given Samvel n boxes indexed from 1 to n. All the boxes except the first one are located in another box. Robert wants to fill the boxes with apples (At beginning boxes contain no apples).&nbsp; Robert can ask Samvel queries of 4 types.</p>
<p>The queries are</p>
<p>1) Robert says two integers x,y to Samvel. Samvel needs to add x (1¡Üx¡Ü10^9) apples to the y-th box. (1¡Üy¡Ün)</p>
<p>2) Robert says two integers x,y to Samvel. Samvel needs to swap the indexes of the x-th and y-th boxes. (1¡Üx,y¡Ün)</p>
<p>3) Robert says an integer x to Samvel. Samvel needs to say the number of apples located in the box x (1¡Üx¡Ün)&nbsp;and in the boxes that are in the box x (directly or indirectly).</p>
<p>4) Robert says an integer x to Samvel. Samvel needs to answer the query of the third type for the box that has minimum index from the boxes that are located directly in the box x. (1¡Üx¡Ün)</p>
<p>Samvel needs your help. help him and write a program to answer this queries.</p>
<h3>Input</h3>
<p>The first line of input contains an integer n (2¡Ün¡Ü10^5)&nbsp; and q (1¡Üq¡Ü10^5), number of boxes and number of queries.</p>
<p>Second line contains n-1 integers a<sub>1</sub>...a<sub>n-1</sub>. a<sub>i-1</sub> is the index of the box that contains box i. (1¡Üa<sub>i</sub>¡Ün)</p>
<p>The lines from 3 to q+2 contain an integer k (type of the query). if k=1 or k=2 then goes the two integer x,y from the task, else there is only one integer x.</p>
<h3>Output</h3>
<p>For each query of type 3 or 4 you need to output one integer the answer of query in a seperate line. If query type is 4 and given box has no oher boxes in it print -1.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
4 6
1 1 2
1 5 1
3 1
2 1 3
3 3
1 60 1
4 3
</pre>
<pre><strong>Output:</strong>
5
5
60
</pre>