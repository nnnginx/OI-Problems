<p><span style="font-size: small;">You are visiting a park which has <strong>N</strong> islands. From each island i, exactly one bridge was constructed.</span> <span style="font-size: small;">The length of that </span><span style="font-size: small;">bridge is denoted by <strong>Li</strong>. The total number of bridges in the island is <strong>N</strong>.</span> <span style="font-size: small;">Each bridge can be traversed in both directions. Also, for each pair of island</span>, <span style="font-size: small;">there is a unique ferry that travels back and forth between them. </span></p>
<p><br><span style="font-size: small;">Since you like walking better than riding ferries, you want to maximize the sum of the lengths of the bridges you cross subject to the constraints below :</span></p>
<ul>
<li><span style="font-size: small;">You can start a visit on an island of your choice.</span></li>
<li><span style="font-size: small;">You may not visit any island more than once.</span></li>
<li><span style="font-size: small;">At any time you may move from your current island S to any island D which you have not visited before. You can go from S to D either by walking, in which case the length of the bridge you take will be added to the total length or by ferry if the islands are not connected by any bridge (when checking for connectivity you should include those islands which have been previously visited by you).</span></li>
</ul>
<p><span style="font-size: small;">Note that you do not have to visit all the islands, and it may be impossible to cross al the bridges.</span></p>
<p><span style="font-size: small;">Given N bridges along with their lengths, your task is to find out the maximum distance you can walk by following the rules above.</span></p>
<p><strong><span style="font-size: small;">Constraints :<br></span></strong></p>
<p><span style="font-size: small;">2 &lt;= N &lt;= 100000</span></p>
<p><span style="font-size: small;">1 &lt;= Li &lt;= 1000000</span></p>
<h2 style="text-align: center;"><span style="font-size: small;"><strong>Input</strong><br></span></h2>
<p><span style="font-size: small;">The first line of the input contains N, the number of islands. Islands are numbered 1 to N inclusive. Then follow N lines. The ith of these lines contains two integers Ii and Li, which are the island the ith island connects to and the length of the bridge respectively. You may assume that each bridge has two different islands as its endpoints.</span></p>
<h2 style="text-align: center;"><span style="font-size: small;"><strong>Output</strong><br></span></h2>
<p><span style="font-size: small;">You must write a single line which is the maximum possible distance that you can walk.</span></p>
<h2 style="text-align: center;"><span style="font-size: small;"><strong>Example</strong><br></span></h2>
<p><strong><span style="font-size: small;">Input :</span></strong></p>
<p><span style="font-size: small;">7</span></p>
<p><span style="font-size: small;">3 8</span></p>
<p><span style="font-size: small;">7 2</span></p>
<p><span style="font-size: small;">4 2</span></p>
<p><span style="font-size: small;">1 4</span></p>
<p><span style="font-size: small;">1 9</span></p>
<p><span style="font-size: small;">3 4</span></p>
<p><span style="font-size: small;">2 3</span></p>
<p><strong><span style="font-size: small;">Output :</span></strong></p>
<p><span style="font-size: small;">24</span></p>
<p><span style="font-size: small;"><strong>Explanation of the example :</strong></span></p>
<p><span style="font-size: small;">Start at 5.</span></p>
<p><span style="font-size: small;">Walk to 1.</span></p>
<p><span style="font-size: small;">Walk to 3.</span></p>
<p><span style="font-size: small;">Walk to 6.</span></p>
<p><span style="font-size: small;">Ferry to 7.</span></p>
<p><span style="font-size: small;">Walk to 2.</span></p>
<p><span style="font-size: small;">Hence total distance you walked is 9 + 8 + 4 + 3 = 24.<br></span></p>
<p><span style="font-size: small;"><strong>Note : </strong>The final answer fits within 64 bit integer.<br></span></p>