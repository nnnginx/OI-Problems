<p><strong>[Due to SPOJ restrictions, this problem has been modified with respect to the original version used in the Argentinian Programming Tournament of 2015 in order to have multiple test cases per input file. The original version of this problem (in Spanish) can be found at <a href="http://torneoprogramacion.com.ar/wp-content/uploads/2015/09/pruebaTAP2015.pdf">http://torneoprogramacion.com.ar/wp-content/uploads/2015/09/pruebaTAP2015.pdf</a>&nbsp;]</strong></p>
<p>Amelia has decided to retire from programming competitions and move to a more peaceful place, away from the noisy city. She dreams of sitting in front of her house to see the sunset over the countryside, while listening on the radio to one of her beloved soap operas. However, before fulfilling her dreams she must solve one last problem, which consists in choosing where she should move.</p>
<p>The countryside where Amelia wants to move to is very large and flat, so much so that it can be represented by an infinite plane on which we imagine a Cartesian coordinate system <strong>(X, Y)</strong>. In this countryside there are <strong>N</strong> radio stations numbered <strong>1</strong> through <strong>N</strong>. The <strong>i</strong>-th radio station transmits its signal from an antenna placed at point <strong>(X<sub>i</sub>, Y<sub>i</sub>)</strong>, having said signal a range of <strong>R<sub>i</sub></strong>. This radio station can be tuned in to from any point <strong>(X, Y)</strong> whose distance to the antenna is less or equal to the corresponding range, <em>i.e.</em> satisfying:</p>
<p style="text-align: center;"><strong>(X - X<sub>i</sub>)<sup>2</sup> + (Y - Y<sub>i</sub>)<sup>2</sup> ≤ R<sub>i</sub><sup>2</sup></strong></p>
<p>The signals from different radio stations can overlap, but will never interfere with each other. In order to listen to as many soap operas as possible, Amelia wants to place her house at some point within the range of the maximum possible number of radio stations. Now Amelia wants to know, given the description of the countryside, what is the maximum number of radio stations she will be able to tune in to as she sees the sunset over the countryside sitting in front of her house.</p>
<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Amelia has decided to retire from programming competitions and move to a more peaceful place, away from the noisy city. She dreams of sitting in front of her house to see the sunset over the countryside, while listening on the radio to one of her beloved soap operas. However, before fulfilling her dreams she must solve one last problem, which consists in choosing where she should move.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The countryside where Amelia wants to move to is very large and flat, so much so that it can be represented by an infinite plane on which we imagine a Cartesian coordinate system (X, Y). In this countryside there are N radio stations numbered 1 through N. The i-th radio station transmits its signal from an antenna placed at point (X[i], Y[i]), having said signal a range of R[i]. This radio station can be tuned in to from any point (X, Y) whose distance to the antenna is less or equal to the corresponding range, i.e. satisfying:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">(X - X[i])² + (Y - Y[i])² ≤ R[i]²</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">
<p>The signals from different radio stations can overlap, but will never interfere with each other. In order to listen to as many soap operas as possible, Amelia wants to place her house at some point within the range of the maximum possible number of radio stations. Now Amelia wants to know, given the description of the countryside, what is the maximum number of radio stations she will be able to tune in to as she sees the sunset ove</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>Amelia has decided to retire from programming competitions and move to a more peaceful place, away from the noisy city. She dreams of sitting in front of her house to see the sunset over the countryside, while listening on the radio to one of her beloved soap operas. However, before fulfilling her dreams she must solve one last problem, which consists in choosing where she should mov</p>
</div>
<h3>Input</h3>
<p>There are multiple test cases in the input file. For each test case, the first line contains an integer <strong>N</strong> representing the number of radio stations in the countryside (<strong>1 ≤ N ≤ 100</strong>). Each of the following <strong>N</strong> lines contains three integers <strong>X<sub>i</sub></strong>, <strong>Y<sub>i</sub></strong> and <strong>R<sub>i</sub></strong> representing respectively the coordinates of the antenna and the range of the <strong>i</strong>-th radio station (<strong>-1000 ≤ X<sub>i</sub>, Y<sub>i</sub>&nbsp;≤ 1000</strong> and <strong>1 ≤ R<sub>i</sub>&nbsp;≤ 1000</strong> for <strong>i = 1, 2, ..., N</strong>).</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>For each test case, print one line containing an integer representing the maximum number of radio stations Amelia will be able to tune in to if she optimally chooses where to move to.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<span style="font-family: 'courier new', courier;">5
-1 0 2
1 0 2
0 -2 1
0 0 1
0 2 1</span>

<strong>Output:</strong>
<span style="font-family: 'courier new', courier;">4</span></pre>