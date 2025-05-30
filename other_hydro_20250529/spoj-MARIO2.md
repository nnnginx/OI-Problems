<p>Mario usually relaxes himself by walking along the shady track near the Mushroom Kingdom. The evil King Koopa noticed that and placed a lot of mushroom on the road. There are two types of mushrooms, max mushrooms and bad mushrooms. The bad mushrooms will decrease Mario's HP by <strong>m</strong> points, on the other hand, max mushrooms will increase Mario's HP by one point. The mushrooms are randomly placed on the track and Mario will receive them one by one. Once Mario's HP becomes zero or below after he received a mushroom, he will die.</p>
<p>Notice that Mario begins with HP zero, so if the first mushroom is bad, Mario will die immediately. Fortunately, if Mario receives all the mushrooms, he will be alive with HP 1. In the other words, if there are <strong>k</strong> bad mushrooms on the way, there will also be <strong>m</strong>*<strong>k</strong>+1 max mushrooms.</p>
<p>Princess Peach wants to know the possibility for Mario staying alive. Please help her to calculate it out.</p>
<h3>Input</h3>
<p>There are several test cases. The first line contains only one integer denoting the number of test cases.</p>
<p>For each test case, there is only one line including two integers: <strong>m</strong> and <strong>k</strong>, denoting the amount of points of HP the Mario will decrease if he receives a bad mushroom, and the number of bad mushrooms on the track. (1 &lt;= <strong>m</strong> &lt;= 1000, 1 &lt;= <strong>k</strong> &lt;= 1000)</p>
<h3>Output</h3>
<p>For each test case, output only real number denoting the possibility that Mario will survive if he receives all the randomly placed mushrooms one by one. The answer should be rounded to eight digits after the decimal point.</p>
<p><strong>The judge is "ignoring extra white spaces".</strong></p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
1 1
60 80

<strong>Output:</strong>
Case #1: 0.33333333
Case #2: 0.00020488
</pre>