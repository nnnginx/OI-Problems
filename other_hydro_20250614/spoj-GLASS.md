<p>Jozo the glazier has made N square pieces&nbsp;of glass. The dimensions (sides) of these squares are equal to 1, 2, 3, ..., N - therefore, the areas of these squares equal to 1<sup>2</sup>, 2<sup>2</sup>, 3<sup>2</sup>, ..., N<sup>2</sup>.</p>
<p>Four customers have arrived. Each of them buys exactly 3 pieces of of glass (Jozo will therefore sell exactly 12 pieces of glass). Each customer has stated that the sum of the <strong>dimensions</strong>&nbsp;of the squares he gets must be equal to N (for example he could get the pieces with dimensions 1, 2 and N-3).</p>
<p>Furthermore, since all customers pay the same price, Jozo wants to be fair and ensure that the sum of <strong>areas</strong> of the 3 squares must be equal for each customer (but this sum is not defined in advance). Help Jozo to choose which pieces to sell.</p>
<h3>Input</h3>
<p>A natural number N (12 ¡Ü N ¡Ü 1500).</p>
<h3>Output</h3>
<p>Print -1 if there is no solution. Otherwise, print four lines: in each of these four lines there must be three numbers from the set {1, 2, ..., N} and their sum must be equal to N. Also, the sum of squares of these three numbers must be constant for each row. All 12 numbers must be distinct.</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre>84

<strong><strong>Output:</strong></strong></pre>
<pre><div id="_mcePaste" style="font-weight: bold; position: absolute; left: -10000px; top: 250px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">18 29 37</div>17 33 34
18 29 37
19 27 38
22 23 39<strong>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 250px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">19 27 38</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 250px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">22 23 3</div></strong><span style="white-space: normal;">
</span></pre>