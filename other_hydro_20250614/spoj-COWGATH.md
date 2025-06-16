<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Cows have assembled from around the world for a massive gathering. There are N cows, and N−1 pairs of cows who are friends with each other. Every cow knows every other cow through some chain of friendships.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">They had great fun, but the time has come for them to leave, one by one. They want to leave in some order such that as long as there are still at least two cows left, every remaining cow has a remaining friend. Furthermore, due to issues with luggage storage, there are M pairs of cows (ai,bi) such that cow ai must leave before cow bi. Note that the cows ai and bi may or may not be friends.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Help the cows figure out, for each cow, whether she could be the last cow to leave. It may be that there is no way for the cows to leave satisfying the above constraints.</div>
<p>Cows have assembled from around the world for a massive gathering. There are <strong><em>N</em></strong> cows, and <strong><em>N−1</em></strong> pairs of cows who are friends with each other. Every cow knows every other cow through some chain of friendships.</p>
<p>They had great fun, but the time has come for them to leave, one by one. They want to leave in some order such that as long as there are still at least two cows left, every remaining cow has a remaining friend. Furthermore, due to issues with luggage storage, there are <strong><em>M</em></strong> pairs of cows <strong><em>(a<sub>i</sub>,b<sub>i</sub>)</em></strong> such that cow <strong><em>a<sub>i</sub></em></strong> must leave before cow <strong><em>b<sub>i</sub></em></strong>. Note that the cows <strong><em>a<sub>i</sub></em></strong> and <strong><em>b</em></strong><sub><strong><em>i</em></strong>&nbsp;</sub>may or may not be friends.</p>
<p>Help the cows figure out, for each cow, whether she could be the last cow to leave. It may be that there is no way for the cows to leave satisfying the above constraints.</p>
<h3>Input</h3>
<p>Line <strong>1</strong> contains two space-separated integers <em><strong>N</strong></em> and <em><strong>M</strong></em>.</p>
<p>Lines <strong><em>2 ≤ i ≤ N</em></strong> each contain two integers <em><strong>x<sub>i</sub></strong></em> and<strong><em> y<sub>i</sub></em></strong> with <em><strong>1 ≤ x<sub>i</sub>, y<sub>i</sub> ≤ N</strong></em> and <strong>x<sub>i</sub> ≠ y<sub>i</sub></strong> indicating that cows <strong><em>x<sub>i</sub></em></strong> and <strong><em>y<sub>i</sub></em></strong> are friends.</p>
<p>Lines <em><strong>N+1 ≤ i ≤ N+M</strong></em> each contain two integers <strong><em>a<sub>i</sub></em></strong> and <em><strong>b<sub>i</sub></strong></em> with <em><strong>1 ≤ a<sub>i</sub>, b<sub>i</sub> ≤ N</strong></em> and <em><strong>a<sub>i</sub> ≠ b<sub>i</sub></strong></em>&nbsp;indicating that cow <em><strong>a<sub>i</sub></strong></em> must leave the gathering before cow <strong><em>b<sub>i</sub></em></strong>.</p>
<p>It is guaranteed that <strong><em>1 ≤ N, M ≤ 10<sup>5</sup></em></strong>.</p>
<h3>Output</h3>
<p>The output should consist of <em><strong>N</strong></em> lines, with one integer <strong><em>d<sub>i</sub></em></strong> on each line such that <strong><em>d<sub>i&nbsp;</sub>= 1</em></strong> if cow i could be the last to leave, and <strong><em>d<sub>i&nbsp;</sub>= 0</em></strong> otherwise.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5 1
1 2
2 3
3 4
4 5
2 4</pre>
<pre><strong>Output:</strong>
0
0
1
1
1
<span style="white-space: normal;">
</span></pre>