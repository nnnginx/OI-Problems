<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">After many years of art, young Florian wants to work in one conglomerate.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">There are N persons assigned by numbers from 1 to N, of which some interns are. Florijan knows</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">all the interns in this company and fascinated by the massiveness of the hierarchy.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">In the enterprise hierarchy, every employee has a single boss, except the chief boss, ie the director</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">who does not have a boss over himself. There is no cycle within the hierarchy, ie hierarchy is a tree form. Also worth it</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">that a trainee can not be superiors to non-trained employees.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Speaking to practitioners, Florian had collected a wealth of information about the layout of a part of the hierarchy.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Namely, for every intern he learned who his boss was (maybe his boss is also a trainee). Florian</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">now entertains counting the distance of some of the two internships in the hierarchy, which counts as the number of bosses between</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">these internships.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">More precisely, the distance to the hierarchy for two employees is obtained by climbing the hierarchy</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">starting with them, count all their direct and indirect bosses to their first boss (including</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">and him). If one of the observed two employees is supervised by another (directly or indirectly),</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">we only count the bosses who are strictly in the hierarchy between them.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Help young Florian determine the maximum distance of two internships across the hierarchy, if this</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">number can be determined (not interested in exactly the ones who are exactly the most distant).</div>
<p>After many years of art, young Florian wants to work in a conglomerate. This company consists of N employees denoted 1, 2, ..., N, of which some are <strong>interns</strong>. Florian knows all interns in this company. In the hierarchy, every employee has a single boss, except for one employee (the CEO) who does not have a boss. There is no cycle within the hierarchy; in other words, the hierarchy is a tree. Also, <strong>an</strong>&nbsp;<strong>intern cannot be superior to a non-intern</strong>.</p>
<p>Speaking to interns, Florian has collected a wealth of information about <strong>parts</strong> of the hierarchy. Namely, for every intern he knows who his/her boss is (this boss could also be an intern).</p>
<p>Florian now counts the distance of two interns in the hierarchy, which is the number of bosses between these interns. More precisely, the <strong>distance in the hierarchy</strong> between two employees is obtained by climbing the hierarchy starting with them, and counting all their direct or indirect superiors up to their first common superior (including him). If one of the observed two employees is superior to another (directly or indirectly), we only count the employees who are strictly between them in the hierarchy.</p>
<p>Help young Florian determine the <strong>largest distance of two interns</strong> across the hierarchy, if this number can be uniquely determined from the known data.</p>
<h3>Input</h3>
<p>The first line contains two integers N and M, the total number of employees in the company and the number of interns (2 ¡Ü M &lt; N ¡Ü 100 000).</p>
<p>Each of the following M lines contains two integers A and B, intern and his boss (1 ¡Ü A, B ¡Ü N, A ¡Ù B). No intern will have two bosses.</p>
<h3>Input</h3>
<p>Print the required largest intern distance, or -1 if the answer cannot be determined.</p>
<h3>Example</h3>
<table border="0">
<tbody>
<tr>
<td>
<pre><strong>Input:</strong>
5 4
2 1
3 2
4 3
5 4
</pre>
</td>
<td>
<pre><strong>Input:</strong>
7 4
1 2
2 3
4 5
5 6 </pre>
</td>
<td>
<pre><strong>Input:</strong>
3 2
2 1
3 1</pre>
</td>
</tr>
<tr>
<td>
<pre><strong>Output:</strong>
2</pre>
</td>
<td>
<pre><strong>Output:</strong>
-1</pre>
</td>
<td>
<pre><strong>Output:</strong>
1</pre>
</td>
</tr>
</tbody>
</table>