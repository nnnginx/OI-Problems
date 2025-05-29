<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Unexpected problems with law enforcement have convinced Mirko to take up a less lucrative but less</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">morally ambiguous career: he has become the chief organizer of a team computer science contest.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">There are N CS clubs that wish to participate in the contest. The presidents of the clubs are quite</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">stubborn and will participate in the contest only if the contest team size makes it possible for all club</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">members to participate.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The contest consists of two rounds: qualifications and finals. All teams that are competing must have</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">an equal number of members and all members of one team must belong to the same club. Any</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">number of teams from each club can participate in the qualification round, and the best team from</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">each club earns a spot in the finals.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Mirko is aware that, with a new and unproven contest, he needs publicity. For that reason, he wants to</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">set the team size such that the number of individual participants in the finals is as large as possible.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Remember, each club that participates has a right to one team in the finals. Furthermore, at least two</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">clubs must participate in the contest, otherwise the contest would be too boring to attract sponsors.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Determine the maximum possible number of participants in the finals so that Mirko can double check</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">his team size choice.</div>
<p>After Mirko's failed stint as a coach and a passing obsession with Croatian meat delicacies, his weight</p>
<p>problems have motivated him to work hard as a farmer. He has moved to a village where his friend</p>
<p>Slavko lives. Farmers in the village share a large common plot of land in the shape of a N×N square,</p>
<p>divided into N² unit squares. A unit square at coordinates (i, j) brings in the income of Aij, which can</p>
<p>be negative (for example, if the square has to be maintained but is not cultivated). The farmers always</p>
<p>divide the common land into smaller rectangular fields with edges parallel to the common land</p>
<p>edges.</p>
<p>Slavko is skeptical of Mirko since his failure as a coach, so he insists that both of them are assigned</p>
<p>land with the same total income, but also thet the two plots share exactly one common corner so</p>
<p>that the two friends can keep an eye on each other (Slavko knows that Mirko is prone to mischief). The</p>
<p>common corner must be the only point where the two plots meet, in order to prevent border-related</p>
<p>arguments.</p>
<p>You are given a description of the common land plot. Find the total number of plot pairs that satisfy</p>
<p>Slavko's criteria.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>The first line of input contains the positive integer N (1 ≤ N ≤ 50), the dimensions of the common</p>
<p>land plot.</p>
<p>Each of the following N lines contains N space-separated numbers Aij (-1000 &lt; Aij &lt; 1000), the income</p>
<p>provided by the respective cell.</p>
<h3>Output</h3>
<p>The first and only line of output must contain the total number of plot pairs satisfying the given</p>
<p>condition.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3</pre>
<pre>1 2 3</pre>
<pre>2 3 4</pre>
<pre>3 4 8</pre>
<pre><strong>Output:</strong>
7</pre>