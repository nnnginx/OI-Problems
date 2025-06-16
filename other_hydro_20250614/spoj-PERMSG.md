<p>Alice, a permutation aficionado, has thought up a permutation of <strong>N</strong> (1 &lt;= <strong>N</strong> &lt;= 100000) integers in the range [0, <strong>N</strong>-1], <strong>P</strong>.  So impressed with herself she has told her friend Bob about <strong>P</strong>.</p>
<p>Normally Alice would call it a day after creating such an impressive permutation but today she decided that she wanted to raise <strong>P</strong> to the power <strong>k</strong> (a positive integer) as well!  Unfortunately, after working on the problem for a while she gave up because it was taking too long.  Not wanting her efforts to go to waste she once again tells Bob about all the elements she has determined so far.  Unfortunately, she neglected to tell Bob the value <strong>k</strong>.</p>
<p>Bob, very interested in Alice's work, needs your help to try and determine any additional elements of <strong>P</strong>^<strong>k</strong>.  Bob is suspicious of Alice's work so he also asks you to check it for errors.</p>
<h3>Notes</h3>
<p>For two permutations <strong>P</strong>, <strong>Q</strong>, the <strong>i</strong>th element of the product, <strong>(P * Q)[i]</strong>, can be computed as <strong>Q[P[i]]</strong> where arrays are all 0-indexed.</p>
<p>Then <strong>P^k</strong> is simply <strong>P</strong> * <strong>P</strong> * ... <strong>k</strong> times ... * <strong>P</strong>.</p>
<h3>Input</h3>
<p>The first line of input contains <strong>N</strong> (1 &lt;= <strong>N</strong> &lt;= 100000), the number of elements in the permutation.  The next line contains a permutation of the integers 0 through <strong>N</strong>-1 each separated by a space.  The following line will contain the result of applying the permutation <strong>k</strong> times with the exception that elements that are not known will be -1 instead.</p>
<h3>Output</h3>
<p>Print <strong>P</strong>^<strong>k</strong> as a space separated list on its own line with as many elements as possible determined.  If an element can't be determined leave it as -1.  If there is no <strong>k</strong> such that <strong>P</strong>^<strong>k</strong> has the values given in the input print "Inconsistent" (quotes for clarity) on its own line instead.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
4
1 2 3 0
3 -1 -1 -1

<strong>Output:</strong>
3 0 1 2
</pre>
<pre><strong>Note</strong>: The first four permutations generated are

1 2 3 0
2 3 0 1
3 0 1 2
0 1 2 3</pre>
<h3>Example 2</h3>
<pre><strong>Input:</strong>
4
1 2 3 0
3 -1 2 -1

<strong>Output:</strong>
Inconsistent
</pre>