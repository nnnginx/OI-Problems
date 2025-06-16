<p><span style="white-space: normal;">&nbsp;</span></p>
<p>An alien group has attacked Kasukabe so whole city is in big trouble!.All people (count is N) in Kasukabe try to run away so is Shinchan!, they came accross a bridge over a river, and that bridge has been cursed by aliens.Bridge will collapse when someone passes over it.</p>
<p>Shinchan as a legend calls an ultra legend Buri Buri Zaemon by his magic card.Buri Buri appears and suggests shinchan that whenever a person having magic card in his hand&nbsp;passes over the bridge then it will not collapse but since bridge is fragile only maximum 2 persons at a time can pass over it (and one of them should have magic card in his hand) .All citizens of Kasukabe have to go to other side of the river using bridge as quickly as possible.When two persons A and B pass over bridge, it takes MAX(time(A),time(B)) to get them on the other side of river (where time(i) is the time taken by ith person to pass over the bridge).Shinchan has an array of all time[] values of all citizens.</p>
<p>Find the minimum time in which they escape the bridge.(there is only one magic card)</p>
<h3>Input&nbsp;</h3>
<p>first line contains N</p>
<p>1&lt;=N&lt;=100000</p>
<p>Next line contains N integers</p>
<p>1&lt;=time[i]&lt;=1000000000 for each 1&lt;=i&lt;=N</p>
<h3>Output</h3>
<p>Output the minimum time to get all persons over the other side of the river</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
4</pre>
<pre>1 2 5 10

<strong>Output:</strong>
17</pre>
<pre>Description:</pre>
<pre>1 and 2 cross</pre>
<pre>1 comes back</pre>
<pre>5 and 10 cross</pre>
<pre>2 comes back</pre>
<pre>1 and 2 cross</pre>
<pre>Total = 2 +1 + 10 + 2 + 2 =17.</pre>
<pre><div id="_mcePaste" style="position: absolute; left: -10000px; top: 138px; width: 1px; height: 1px; overflow: hidden;">&nbsp; <span style="white-space: pre;"> </span>&nbsp; |&nbsp; &nbsp; &nbsp; &nbsp;|</div>(here persons are denoted by there crossing time.)
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 138px; width: 1px; height: 1px; overflow: hidden;">1,2,5,10&nbsp; &lt;-------&gt;&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 138px; width: 1px; height: 1px; overflow: hidden;"><span style="white-space: pre;"> </span>&nbsp; <span style="white-space: pre;"> </span>total= 17</div></pre>