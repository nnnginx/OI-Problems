<p>This is a very ad-hoc problem. Consider a sequence (N, N-1, ..., 2, 1). You have to reverse it, that is, make it become (1, 2, ..., N-1, N). And how do you do this? By making operations of the following kind.</p>
<p>Writing three natural numbers A, B, C such that 1 ¡Ü A ¡Ü B &lt; C ¡Ü N means that you are swapping the block (block = consecutive subsequence) of elements occupying positions A...B with the block of elements occupying positions B+1..C. Of course, the order of elements in a particular block does not change.</p>
<p>This means that you can pick any two adjacent blocks (each of an arbitrary length) and swap them. The problem can easily be solved in N-1 operations, but to make it more difficult, you must think of a faster way.</p>
<h3>Input</h3>
<p>A natural number 1 &lt; N &lt; 100.</p>
<h3>Output</h3>
<p>Output at most 50 operations, one per line. Each opearations is represented by three numbers as described above.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5

<strong>Output:</strong>
2 3 5</pre>
<pre>1 2 4</pre>
<pre>2 3 5</pre>
<pre><pre style="color: #000000; font-family: Verdana, Arial, Helvetica, sans-serif; font-size: 10px; margin: 8px;"><strong>Explanation of the sample output:</strong> (5 4 3 2 1) --&gt; (5 2 1 4 3) --&gt; (1 4 5 2 3) --&gt; (1 2 3 4 5)</pre>
</pre>