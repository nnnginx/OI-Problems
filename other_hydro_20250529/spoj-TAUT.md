<p>
Write a program that checks if the given logical expression is a tautology. The logical expression is a tautology if it is always true, regardless of logical value of its variables.
</p>

<h3>Input</h3>
<p>
On the first line there is the number of expressions to check (at most 35). The expression is in a prefix notation, that means that operator precedes its arguments. The following logical operators will be used:
</p>
<pre>C - and 
D - or
I - implies
E - if, and only if
N - not
</pre>
<p>
The variables will be lowercase letters (a-z). There will be no more than 16 different letters in the expression. The length of the expression will not exceed 111 characters. 
</p>

<h3>Output</h3>
<p>
For each expression write one word: YES if it is a tautology, NO in other case.
</p>

<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
7
IIpqDpNp
NCNpp
Iaz
NNNNNNNp
IIqrIIpqIpr
Ipp
Ezz


<b><tt>Sample output:</tt></b>
YES
YES
NO
NO
YES
YES
YES
</pre>