<p>You are provided with a sequence of parentheses, that are balanced. A balanced parantheses sequence it that sequence in which every opening bracket has a unique closing bracket (nearest to it) to the right of it and every closing bracket has a unique opening bracket to the left of it (nearest). Any other sequence is not balanced. For example, (()), ()(), ((()())()), (), etc are balanced, but )(), ()), (()(, ()( are unbalanced.</p>
<p>You are then provided with q queries, i<sup>th</sup> query is of form x<sub>i</sub>,&nbsp;, representing an index. the bracket at that index is fliiped that is, if it was an opening bracket then it is replaced by a closing one and vice versa. You have to give the left most index whose bracket has to be flipped so that the sequence remains balanced. <strong>The subsequent queries have to be applied on new sequence formed!&nbsp;</strong></p>
<h3>&nbsp;Input</h3>
<p>The first line will contain two integers, n and q. Next line will give you the sequence (n characters) consisting of opening and closing parenthesis only. Next q lines will represent q queries, x<sub>i</sub>.</p>
<h3>Output</h3>
<p>For each query, output the required answer in different lines.</p>
<h3>Constraints</h3>
<p>1&lt;=n&lt;=4*10^5</p>
<p>1&lt;=q&lt;=2*10^5</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
10 10
()(((())))
2
7
9
4
5
1
4
3
5
4

<strong>Output:</strong>
2
4
6
4
2
1
2
2
4
4

<strong>Input:</strong>
6 9
((()))
6
2
2
6
4
6
3
2
4


<strong>Output:</strong>
6
2
2
6
2
6
2
2
3
</pre>