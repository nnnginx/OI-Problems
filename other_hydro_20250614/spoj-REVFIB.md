<p>The well-known Fibonacci sequence is defined as following:</p>
<p><img src="../../../content/john_jones:revfib.jpg" alt=""></p>
<p>Here we regard n as the index of the Fibonacci number F(n).</p>
<p>This sequence has been studied since the publication of Fibonacci's book <em>Liber Abaci</em>. So far, many properties of this sequence have been introduced.</p>
<p>You had been interested in this sequence, while after reading lots of papers about it. You think there's no need to research in it anymore because of the lack of its unrevealed properties. Yesterday, you decided to study some other sequences like Lucas sequence instead.</p>
<p>Fibonacci came into your dream last night. "Stupid human beings. Lots of important properties of Fibonacci sequence have not been studied by anyone, for example, from the Fibonacci number 347746739��"</p>
<p>You woke up and couldn't remember the whole number except the first few digits Fibonacci told you. You decided to write a program to find this number out in order to continue your research on Fibonacci sequence.</p>
<h3>Input</h3>
<p>There are multiple test cases. The first line of input contains a single integer T denoting the number of test cases (T&lt;=50000).</p>
<p>For each test case, there is a single line containing one non-empty string made up of at most 40 digits. And there won't be any unnecessary leading zeroes.</p>
<h3>Output</h3>
<p>For each test case, output the smallest index of the smallest Fibonacci number whose decimal notation begins with the given digits. If no Fibonacci number with index <strong>smaller than</strong> 100000 satisfy that condition, output -1 instead �C you think what Fibonacci wants to told you beyonds your ability.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
15
1
12
123
1234
12345
9
98
987
9876
98765
89
32
51075176167176176176
347746739
5610

<strong>Output:</strong>
Case #1: 0
Case #2: 25
Case #3: 226
Case #4: 1628
Case #5: 49516
Case #6: 15
Case #7: 15
Case #8: 15
Case #9: 43764
Case #10: 49750
Case #11: 10
Case #12: 51
Case #13: -1
Case #14: 1233
Case #15: 22374
</pre>
<p><em>This problem is first solved by team </em><strong>Y.E.S</strong> (Tsinghua University) <em>at 77 minutes after the onsite contest starts. (They have 2 wrong tries before they get Accepted.)</em></p>
<p>&nbsp;</p>