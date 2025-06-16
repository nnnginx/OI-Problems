<p>Given two strings A and B, we define the operator ĉ on {A,B} for string C as C ĉ {A,B}.
</p><pre>if length(A) &lt; length(C) &lt; length(B), then C satisfies the above operator.
else
      if length(A)=length(C), then C must be lexicographically greater than A.
      if length(B)=length(C), then C must be lexicographically smaller than B.
</pre> 

<h3>Input</h3>
<p>Given two strings A,B with length(A) &lt; = length(B) &lt;= 6.  A,B can contain any characters between A and J (capital letters).

</p><h3>Output</h3>
<p>Print the number of strings satisfying the above criteria.
C must also satisfy criteria of A and B. Any two adjacent
characters in string C may neither be the same nor consecutve (i.e. the absoulte difference between the ASCII values of adjacent characters is greater than 1). 

</p><h3>Example</h3>

<pre><b>Input:</b>
A J
AA BCD
ABC DEFG

<b>Output:</b>
8
129
1770

</pre>