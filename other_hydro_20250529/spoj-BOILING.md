<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The trick to boiling vegetables is to make sure all</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">pieces are about the same size. If they are not, the small</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">ones get too soft or the large ones get undercooked (or</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">both). Fortunately, you have heard of the kitchen knife,</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">but your parents’ warnings of using sharp instruments</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">still echoes in your head. Therefore you better use it as</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">little as possible. You can take a piece of a vegetable of</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">weight w and cut it arbitrarily in two pieces of weight</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">wleft and wright, where wleft + wright = w. This operation</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">constitutes a “cut”. Given a set of pieces of vegetables,</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">determine the minimum number of cuts needed to make the ratio between the smallest and the</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">largest resulting piece go above a given threshold.</div>
<p>The trick to boiling vegetables is to make sure all pieces are about the same size. If they are not, the small ones get too soft or the large ones get undercooked (or both). Fortunately, you have heard of the kitchen knife, but your parents’ warnings of using sharp instruments still echoes in your head. Therefore you better use it as little as possible. You can take a piece of a vegetable of weight w and cut it arbitrarily in two pieces of weight w<sub>left</sub> and w<sub>right</sub>, where w<sub>left</sub> + w<sub>right</sub> = w. This operation constitutes a “cut”. Given a set of pieces of vegetables, determine the minimum number of cuts needed to make the ratio between the smallest and the largest resulting piece go above a given threshold.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>The input starts with a ﬂoating point number T with 2 decimal digits, 0.5 &lt; T &lt; 1, and a positive integer N&nbsp;<span style="font-family: 'Helvetica Neue', Helvetica, Arial, san-serif; font-size: 13px; line-height: 16.25px;">≤</span> 1 000. Next follow N positive integer weights w<sub>1</sub>, w<sub>2</sub>, ..., w<sub>N</sub>. All weights are less than 10<sup>6.</sup></p>
<h3>Output</h3>
<p>Output the minimum number of cuts needed to make the ratio between the resulting minimum weight piece and the resulting maximum weight piece be above T. You may assume that the number of cuts needed is less than 500.</p>
<p>To avoid issues with ﬂoating point numbers, you can assume that the optimal answer for ratio T is the same as for ratio T + 0.0001.</p>
<h3>Example</h3>
<pre><strong>Input 1:</strong>
0.99 3
2000 3000 4000

<strong>Output 1:</strong>
6<span style="white-space: normal;">
</span></pre>
<pre><strong>Input 2:</strong>
0.80 2
1000 1400

<strong>Output 2:</strong>
3</pre>