<p>You are given a matrix M of type 1234x5678. It is initially filled with  integers 1...1234x5678 in row major order. Your task is to process a  list of commands manipulating M. There are 4 types of commands: <br> "R x y" swap the x-th and y-th row of M ;<br> "C x y" swap the x-th and y-th column of M ;<br> "Q x y" write out M(x,y) ;<br> "W z" write out x and y where z=M(x,y).</p>
<h3>Input</h3>
<p>A list of valid commands. Input terminated by EOF.</p>
<h3>Output</h3>
<p>For each "Q x y" write out one line with the current value of M(x,y), for each "W z" write out one line with the value of x and y ( interpreted as above ) separated by a space.</p>
<pre><strong>Input:</strong>
R 1 2
Q 1 1
Q 2 1
W 1
W 5679
C 1 2
Q 1 1
Q 2 1
W 1
W 5679

<strong>Output:</strong>
5679
1
2 1
1 1
5680
2
2 2
1 2
</pre>