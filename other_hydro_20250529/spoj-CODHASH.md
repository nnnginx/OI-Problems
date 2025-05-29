<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">There are n cards arranged in a row.The rth card from the left has rth prime number written on it on one side the other side is blank.Some cards have the blank side up and the others have the number side up.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Cards with their blank side up are known as 0-cards and cards showing the prime numbers are known as 1-cards</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">A hash code is generated from the set of cards in the following way:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Initial value of hashcode is 1.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">All the 0-cards should be turned upside down to convert them to a 1-card in order to get the final value of hash code.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp;At each step a 0-card can be turned upside down if there's at least one 1-card adjacent to it.Once the card is turned the value of the hash code is changed &nbsp;according to the following equation:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">new value of hashcode=(previous value of hashcode )*((number on the card)^(number of 0-cards left on the table+1))</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Once all the cards on the table are 1-cards we get the final value of hash code.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Find the total number of distinct hash codes that can be generated for the given arrangement of cards.</div>
<p>There are n cards arranged in a row.The rth card from the left has rth prime number written on it on one side the other side is blank.Some cards have the blank side up and the others have the number side up.</p>
<p>Cards with their blank side up are known as 0-cards and cards showing the prime numbers are known as 1-cards</p>
<p>A hash code is generated from the set of cards in the following way:</p>
<p>Initial value of hashcode is 1.</p>
<p>All the 0-cards should be turned upside down to convert them to a 1-card in order to get the final value of the hash code.</p>
<p>At each step a 0-card can be turned upside down if there's at least one 1-card adjacent to it.Once the card is turned the value of the hash code is changed &nbsp;according to the following equation:</p>
<p>New value of hashcode=(Previous value of hashcode )*((Number on the card)^(Number of 0-cards left on the table+1))</p>
<p>Once all the cards on the table are 1-cards we get the final value of hash code.</p>
<p>Find the total number of distinct hash codes that can be generated like this for the given arrangement of cards.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>The first line contains 0&lt;T&lt;=1000 (T-number of test cases)</p>
<p>The first line of every test case contains two integers n and m where n is the number of cards on the table and m is the number of 1-cards on the table, (1 ≤ n ≤ 1000, 1 ≤ m ≤ n). The second line contains m distinct integers, each between 1 to n inclusive, denoting the indices of the cards that are 1-cards.</p>
<h3>Output</h3>
<p>For every test case print in a separate line&nbsp;the number of &nbsp;distinct hash codes that can be generated for the given arrangement of cards modulo 1000000007 (10^9 + 7).</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2</pre>
<pre>3 1</pre>
<pre>1</pre>
<pre>4 2</pre>
<pre>1 4

<strong>Output:</strong>
1</pre>
<pre>2</pre>