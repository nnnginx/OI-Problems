<p>As you might already know, Ada the Ladybug is a farmer. She has multiple furrows in which she grows vegetables. She also never grows multiple vegetables of the same kind in the same furrow. Ada sometime palnts a new vegetable, harveest a vegetable or asks for some aspect which two different furrows have in common (described in input).</p>
<h3>Input</h3>
<p>The first line of input will contain <strong> 1 ¡Ü Q ¡Ü     3*10<sup>5</sup></strong>, the number of queries.</p>
<p>Each of the next <strong>Q</strong> lines will contain <strong>? x y</strong>: <strong>0 ¡Ü x, y     ¡Ü 2*10<sup>4</sup></strong>, and <strong>?</strong> is one of: <strong>+ - v ^ ! \</strong> with following meaning:</p>
<p>+: Plants vegetable of kind <strong>y</strong> to furrow number <strong>x</strong> (note that there will never be multiple vegetables of the same kind in the same furrow)</p>
<p>-: Harvests vegetable of kind <strong>y</strong> from furrow number <strong>x</strong> (note that there will always be a vegetable of that kind)</p>
<p>v: Finds out how many kinds of vegetables there are in furrows <strong>x</strong> and <strong>y</strong>.</p>
<p>^: Finds out how many kinds of vegetable are in both furrows (<strong>x, y</strong>)</p>
<p>!: Find out how many kinds of vegetables are in <strong>x</strong> and <strong>y</strong> <strong>BUT</strong> not in both of them at once.</p>
<p>\: Find out how many kinds of vegetable are in <strong>x</strong> but not in <strong>y</strong></p>
<h3>Output</h3>
<p>For each query of the last four kinds, output the proper answer.</p>
<h3>Example Input</h3>
<pre>10
+ 1 4
! 0 2
+ 0 2
\ 0 2
^ 0 1
v 2 0
+ 2 4
! 2 0
+ 1 0
! 0 2</pre>
<pre><span style="font-size: 1.17em;">Example Output</span>
</pre>
<pre>0
1
0
1
2
2
</pre>
<h3>Example Input</h3>
<pre>15
+ 0 2
! 0 1
+ 1 1
v 0 1
+ 1 2
! 1 0
! 0 1
+ 0 0
v 0 1
^ 0 1
+ 1 3
\ 1 0
\ 1 0
+ 1 0
- 1 2
</pre>
<h3>Example Output</h3>
<pre>1
2
1
1
3
1
2
2
</pre>
<h3>Example Input</h3>
<pre>10
+ 2 1
! 3 1
! 3 1
+ 1 1
\ 2 0
+ 3 1
v 2 3
! 2 3
- 1 1
^ 1 2

</pre>
<h3>Example Output</h3>
<pre>0
0
1
1
0
0
</pre>