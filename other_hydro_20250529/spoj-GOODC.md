<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>The ACM-ICPC World Finals have begun! However, let's not be too hasty - even though The Team features three of the best coders to have ever coded, they know the importance of first determining <em>what</em> to code.</p>
<p>The contest features $N$ ($1 \leq N \leq 10^6$) problems (conveniently numbered $1..N$), and runs for $M$ ($1 \leq M \leq 10^6$) minutes. Every problem is associated with a distinct colour - and each time a team solves a problem, they receive a balloon of its corresponding colour, which is visible to all. Obviously, easier problems will be solved by more teams, and so more of their balloons will be floating around in the contest room. Additionally, The Team has found that earlier problems in the set tend to be easier. Therefore, given 2 problems $i$ and $j$, $i$ is considered easier than $j$ if there are either more $i$ balloons than $j$ balloons in the room, or there are an equal number of balloons and $i&lt;j$.</p>
<p>At the start of the contest (at the 0th minute), there are no balloons in the room, of course. After that, during every minute $i$ (for $i=1..M$), problem $p_i$ ($1 \leq p_i \leq N$) is either solved by The Team (which will only happen if they have not solved it previously), or by some opposing team. The former possibility is represented by $t_i=1$, and the latter by $t_i=2$. In either case, a $p_i$ balloon is brought into the room. However, in the former case, The Team will no longer care about problem $p_i$ in the slightest.</p>
<p>At the end of every minute after the 0th one, the members of The Team want to get their bearings on what they should be working on (and what they should be staying away from). Specifically, out of problems that they haven't yet solved, they want to know what the single easiest and the single hardest problems are, given the information that can be gleaned from the balloons. These two values may be the same, if The Team has only one problem left to solve. If they're solved all of the problems already, they can instead commence the process of making distracting noises. Are you smart enough to figure out what The Team's strategy throughout the contest will be?</p>
<p><span style="font-size: 1.17em;"><strong>Input</strong></span></p>
<p>First line: 2 integers, $N$ and $M$</p>
<p>Next $M$ lines: 2 integers, $t_i$ and $p_i$, for $i = 1..M$</p>
<p><span style="font-size: 1.17em;"><strong>Output</strong></span></p>
<p>$M$ lines: Either 2 integers, the easiest followed by the hardest unsolved problem number after the first $i$ minutes, or the string "Make noise" if all problems have bee solved by The Team, for $i = 1..M$.</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">3 8
2 2
2 1
1 1
2 3
2 3
1 2
1 3
2 1</span></pre>
<pre><strong>Output:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">2 3
1 3
2 3
2 3
3 2
3 3
Make noise
Make noise</span><span style="white-space: normal;">
</span></pre>
<pre><strong>Explanation of Sample:</strong></pre>
<p>After the first minute, we've seen 1 balloon for problem 2, and 0 balloons for problems 1 and 3. Therefore, the easiest problem is 2, since it has the most balloons, and the hardest problem is 3, since it's the last problem with the least balloons.</p>
<p>After the second minute, the counts for the 3 problems are 1, 1, and 0. The easiest problem is now 1, since it's the first problem with the most balloons, while the hardest is still 3.</p>
<p>After the third minute, the counts for the 3 problems are 2, 1, and 0, but problem 1 has now been solved by The Team. The easiest remaining problem is 2, and the hardest is 3.</p>
<p>After the fourth minute, the counts for the 3 problems are 2 (solved), 1, and 1. The easiest unsolved problem is 2, and the hardest is 3.</p>
<p>After the fifth minute, the counts for the 3 problems are 2 (solved), 1, and 2. The easiest unsolved problem is 3, and the hardest is 2.</p>
<p>After the sixth minute, the counts for the 3 problems are 2 (solved), 2 (solved), and 2. The only unsolved problem is 3.</p>
<p>After the seventh and eighth minutes, all 3 problems have been solved by The Team, so noise should be made.</p>