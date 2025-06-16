<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/SPACESET/en/">English</a></td> 
<td width="50%"><a href="/problems/SPACESET/vn/">Vietnamese</a></td> 
</tr></tbody></table>


<p>A long time ago in a galaxy far far away ... The empire has built a grand new space colony. This colony has m levels and each level consists of n settlements. Space settlements are connected by routes along which spacecrafts fly. </p>
<p>A level is a ring shaped construction with the n space settlements lying on it. The ring provides routes for the spacecrafts. Within a level, travelling is only possible along the ring. The ring shaped route will be present irrespective of the number of settlements in the level.</p> 
<p>Levels are organised in a heirarchy. Excellent connectivity is provided between levels. Each settlement in a level is connected by a route to every settlement in the levels immediately above and below it. The topmost and the bottom-most levels are also connected in a similar fashion.</p> 
<p>Our adventurous space pilot -- Han Solo wants to ferry people between space settlements. Solo's spacecraft can navigate a path having exactly k stops, no more no less.</p>
<p>Given the values of k, n and m you have to find the number of paths in the space colony that he can use for his work.</p>
<b>Notes:</b>
<ul>
<p>1. A settlement can be visited any number of times in a journey.</p>
<p>2. A path is considered as a sequence of vertices such that there is an edge between consecutive vertices. Two path's are considered to be different if they differ in any one vertex.</p>
<p>3. The topmost and bottom-most levels are connected only if they are different.</p>
<p>4. Image for clarification</p>
<img src="./24407/file/m5KEHOFh.png">
<p>Here the black dots represent the settlements. The connections are showm as rings and lines. </p>
</ul>
<h3>Input</h3>
<p>First line of input contains T, the number of test cases. Every test case will contain the values of m, n and k. 

</p><h3>Output</h3>
<p>Output contains T lines, one for each test case. Every line will consist of the total number of routes possible mod 12345678. 

</p><h3>Example</h3>

<pre><b>Input:</b>
5
1 1 1
1 2 1
3 3 56
4 3 4
691 60 97764

<b>Output:</b>
1
2
8019378
6144
470730 
</pre>

<h3>Constraints</h3>
<p>Dataset 1: T ¡Ü 100, m ¡Ü 1000, n ¡Ü 1000, k ¡Ü 100000 Time limit: 5s   </p>
<p>Dataset 2: T ¡Ü 100, m ¡Ü 10^8, n ¡Ü 10^8, k ¡Ü 10^8 Time limit: 5s  </p>