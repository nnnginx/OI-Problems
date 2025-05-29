<h3>Problem</h3>
<p>Now that you have won Code Jam and been hired by Google as a software engineer, you have been assigned to work on their wildly popular programming contest website.</p>
<p>Google is expecting a lot of participants (<strong>P</strong>) in Code Jam next year, and they want to make sure that the site can support that many people at the same time. During Code Jam 2010 you learned that the site could support at least <strong>L</strong> people at a time without any errors, but you also know that the site can't yet support <strong>P</strong> people.</p>
<p>To determine how many more machines you'll need, you want to know within a factor of <strong>C</strong> how many people the site can support.  This means that there is an integer <strong>a</strong> such that you know the site can support <strong>a</strong> people, but you know the site can't support <strong>a</strong> * <strong>C</strong> people.</p>
<p>You can run a series of <em>load tests</em>, each of which will determine whether the site can support at least <strong>X</strong> people for some integer value of <strong>X</strong> that you choose. If you pick an optimal strategy, choosing what tests to run based on the results of previous tests, how many load tests do you need in the worst case?</p>
<h3>Input</h3>
<p>The first line of the input gives the number of test cases, <strong>T</strong>.  <strong>T</strong> lines follow, each of which contains space-separated integers <strong>L</strong>, <strong>P</strong> and <strong>C</strong> in that order.</p>
<h3>Output</h3>
<p>For each test case, output one line containing "Case #x: y", where x is the case number (starting from 1) and y is the number of load tests you need to run in the worst case before knowing within a factor of <strong>C</strong> how many people the site can support.</p>
<h3>Limits</h3>
<p>1 �� <strong>T</strong> �� 1000.<br> 2 �� <strong>C</strong> �� 10.<br> <strong>L</strong>, <strong>P</strong> and <strong>C</strong> are all integers.</p>
<h4>Small dataset</h4>
<p>1 �� <strong>L</strong> &lt; <strong>P</strong> �� 10<sup>3</sup>.</p>
<h4>Large dataset</h4>
<p>1 �� <strong>L</strong> &lt; <strong>P</strong> �� 10<sup>9</sup>.</p>
<p>Input</p>
<p><code>4<br> 50 700 2<br> 19 57 3<br> 1 1000 2<br> 24 97 2</code></p>
<p>Output</p>
<p><code>Case #1: 2<br> Case #2: 0<br> Case #3: 4<br> Case #4: 2</code></p>
<h4>Explanation</h4>
<p>In Case #2, we already know that the site can support between 19 and 57 people. Since those are a factor of 3 apart, we don't need to do any testing.</p>
<p>In Case #4, we can test 48; but if the site can support 48 people, we need more testing, because 48*2 &lt; 97. We could test 49; but if the site can't support 49 people, we need more testing, because 24 * 2 &lt; 49. So we need two tests.</p>