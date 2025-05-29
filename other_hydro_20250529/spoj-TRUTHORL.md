<!--Converted with LaTeX2HTML 96.1 (Feb 5, 1996) by Nikos Drakos (nikos@cbl.leeds.ac.uk), CBLU, University of Leeds -->


<title>Truth Or Lie</title>



<h2><font color="#0070E8"><a name="SECTION0001002000000000000000">Problem</a></font></h2>

<p>Suppose you have <b>m</b> yes or no questions that you want to ask <b>n</b> people.  You are allowed to ask each person exactly
two different questions.  He/she will answer exactly one of them correctly and one of them incorrectly, you don't know which
is a correct answer and which is an incorrect one. Given their answers, determine the number of combinations of answers to the <b>m</b>
questions that can still be correct (i.e., no contradictions).</p><p>

</p><h2><font color="#0070E8"><a name="SECTION0001003000000000000000">The Input</a></font></h2>
<p>
First line is the number of inputs.
For each set of input, start out with a line of  <b>n&lt;=10000</b> and <b>m&lt;=200</b>, followed by <b>n</b> lines.
The i-th line has four integers <b>a b c d</b>.  It means that the answer given by the i-th person for question a is b, and for question c is d.
Moreover, the answer "1" means yes, and "0" means no.

</p><h2><font color="#0070E8"><a name="SECTION0001004000000000000000">The Output</a></font></h2>
<p>
For each line of input, output "No Inference" if the answers do not help you eliminate any wrong combination
of answers or the number of combinations of possible answers is 0, otherwise output the size of the set of combinations of answers still possible.

</p><h2><font color="#0070E8"><a name="SECTION0001005000000000000000">Sample Input</a></font></h2>
<p>
</p><pre>2
2 2
1 1 2 0
1 1 2 1
4 4
1 1 2 1
1 1 3 0
2 1 4 1
3 1 4 0
</pre>
<p>
</p><h2><font color="#0070E8"><a name="SECTION0001006000000000000000">Sample Output</a></font></h2>
<p>
</p><pre>No Inference
2
</pre>