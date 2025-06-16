<p>
In the prime factorization of a number <strong><em>N</em></strong>, there's two kinds of powers.
Even powers, in red, are psychotic ones, and odd powers, in blue, are ordinary ones.<br>
We'll say <strong><em>N</em></strong> a <strong>Psycho</strong> number if the count of even powers is
strictly greater than the count of odd powers, else an <strong>Ordinary</strong> number.<br>
For example, if <strong><em>N</em> = 67500</strong> with prime factorization 
67500 =
<span style="color:red"> 2<sup>2</sup></span>
 x 
<span style="color:blue"> 3<sup>3</sup></span>
 x 
<span style="color:red"> 5<sup>4</sup></span>
. <br>
 This number have 2
<span style="color:red"> even powers</span>
 and 1 
<span style="color:blue">  odd power</span>.
Since 2&gt;1, so the number 67500 is a Psycho Number.
</p>

<h3>Input</h3>
<p>The first line of input contains an integer
 <strong><em>T</em></strong>, the number of test cases.</p>

<p> Each of the next <strong><em>T</em></strong> lines contains
 one integer <strong><em>N</em></strong>.</p>

<h3>Output</h3>
<p>For each test case, print if <strong><em>N</em></strong> is Psycho or Ordinary number.
</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
2
3
4

<strong>Output:</strong>
Ordinary Number
Psycho Number

</pre>

<h3>Constraints</h3>
<pre>0 &lt; T &lt; 10^4
1 &lt; N &lt; 10^14
</pre>
<p>Time limit is ¡Á2 my top speed with Python3 language, it could be not easy with slow languages.<br>
O(N^.5 / log(N)) should give TLE even with fast languages. You are awaited to submit something between O(N^0.33 / log(N)) and O(N^0.25 / log(N)).
You can try before the quite similar "tutorial" problem : <a href="http://www.spoj.com/problems/PSYCHON/">Psycho</a> before.<br>
@speed addicts : my top C timing is 0.02s. (TL updated 2017-02-11 ; compiler changes)</p>