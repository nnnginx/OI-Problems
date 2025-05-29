<p>Fred Faculty and Paul Power love big numbers. Day after day Fred chooses a random integer <em>n</em> and he computes <em>n!</em>. His friend Paul amuses himself by computing several powers of his randomly chosen integer <em>k</em> like <em>k<sup>2</sup></em>, <em>k<sup>3</sup></em> and so on. On a hot summer day, Fred and Paul got really, really bored, so they decided to play a joke on their buddy Dave Divider. Fred chooses a random integer <em>n</em> while Paul chooses a random integer <em>k</em>. They want Dave to find the biggest integer <em>i</em> such that <em>k<sup>i</sup></em> divides <em>n!</em> without a remainder, otherwise they will throw a cake in Dave's face. Because Dave does not like cakes in his face, he wants you to help him finding that integer <em>i</em>.</p>
<h3>Input</h3>
<p>The first line contains the number of test cases <em>t</em> (<em>1 ¡Ü t ¡Ü 100</em>). Each of the following <em>t</em> lines contains the two numbers <em>n,k</em> (<em>2 ¡Ü n ¡Ü 10<sup>18</sup></em>, <em>2 ¡Ü k ¡Ü 10<sup>12</sup></em>) separated by one space.</p>
<h3>Output</h3>
<p>For each test case, print the maximum integer <em>i</em> on a separate line.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
5 2
10 10

<strong>Output:</strong>
3
2
</pre>
<hr>
<p><strong>Be careful with overflows in this problem (use 64 bit integers, avoid multiplications which will lead to overflow).</strong></p>