<p>Given an array <strong>A</strong> of <strong>k</strong><em><strong> </strong></em>integers (not necessarily distinct), we define the <em>descending alternating sum </em>of this array, denoted <strong>F(A)</strong> the following way. First, we sort the array in descending order. Suppose the elements, after sorting, are <strong>A<sub>1</sub></strong> ¡Ý <strong>A<sub>2</sub></strong> ¡Ý ... ¡Ý <strong>A<sub>k</sub></strong> respectively. Then the descending alternating sum of array <strong>A</strong> is <strong></strong></p>
<p style="text-align: center;"><strong>F(A) =</strong> <strong>A<sub>1</sub> - A<sub>2</sub> + A<sub>3</sub> - ... + (-1)<sup>k+1</sup> A<sub>k</sub></strong>.</p>
<p>For example, if <strong>A = [5, -3, 8, 2, 0, -5] </strong>then after sorting it in descending order, we find <strong>A = [8, 5, 2, 0, -3, -5]</strong>. So the descending alternating sum of this array is <strong>8 - 5 + 2 - 0 + (-3) - (-5) = 7</strong>. In particular, the descending alternating sum of an empty array is <strong>0</strong>.</p>
<p>You are given an array <strong>A</strong> of <strong>n </strong>integers where <strong>1 ¡Ü n ¡Ü 10<sup>5</sup> </strong>and <strong>|A<sub>i</sub>| ¡Ü 10<sup>18</sup></strong>. You have to print the sum of the descending alternating sums of all subsets of this array <strong>A</strong> (there are <strong>2</strong><sup><strong>n</strong></sup> of them) modulo <strong>M = 10<sup>9</sup> + 7</strong>. In other words, if the subsets of array <strong>A</strong> are <strong>S<sub>1</sub>, S<sub>2, </sub>..., S<sub>2<sup>n</sup></sub> </strong>then you have to print the sum</p>
<p style="text-align: center;"><strong>F(<strong>S<sub>1</sub>) + F(<strong>S<sub>2</sub>) + ... + F(<strong>S<sub>2<sup>n</sup></sub>) </strong></strong></strong></strong>modulo <strong>M =<strong> <strong>10<sup>9</sup> + 7</strong></strong></strong>.</p>
<p>Note: we consider some integer modulo a positive integer to be non-negative. In the other words, the output <strong>R </strong>must satisfy the inequality <strong>0 ¡Ü</strong> <strong>R &lt; M</strong>.</p>
<h3>Input</h3>
<p>The first line of the input file contains a single integer <strong>n</strong>, denoting the size of the array <strong>A</strong>.</p>
<p>The second line contains <strong>n </strong>integers <strong>A<sub>1</sub>, A<sub>2</sub>, ..., A<sub>n</sub></strong>, the elements of the array <strong>A</strong>.</p>
<h3>Output</h3>
<p>Print a single integer, the sum of descending alternating sums of all subsets of the array <strong>A</strong>.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3
-1 9 3<br>
<strong>Output:</strong>
36</pre>