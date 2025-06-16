<p>Given
two strings of lowercase letters, <b style=""><i>a</i></b>
and <b style=""><i>b</i></b>, print the longest
string <b style=""><i>x</i></b> of lowercase letters
such that there is a permutation of <b style=""><i>x</i></b>
that is a subsequence of <b style=""><i>a</i></b>
and there is a permutation of <b style=""><i>x</i></b>
that is a subsequence of <b style=""><i>b</i></b>. 

</p><h3>Input</h3>

<p>Input file contains several lines of input.
Consecutive two lines make a set of input. That means in the input file line <b style="">1</b> and <b style="">2</b> is a set of input, line <b style="">3</b>
and <b style="">4</b> is a set of input and so on.
The first line of a pair contains <b style=""><i>a</i></b>
and the second contains <b style=""><i>b</i></b>.
Each string is on a separate line and consists of at most <b style="">1000</b> lowercase letters.

</p><h3>Output</h3>

<p>For each set of input, output a line containing <b style=""><i>x</i></b>. If several <b style=""><i>x</i></b> satisfy the criteria above,
choose the first one in alphabetical order. 

</p><h3>Example</h3>

<pre><b>Sample input:</b>
pretty
women
walking
down
the
street
 
<b>Sample output:</b>
e
nw
et 
</pre>