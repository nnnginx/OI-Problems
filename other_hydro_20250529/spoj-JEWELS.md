<p>You work for a small jewelers' company, renowned for the exquisite necklaces and multi-colored amber strings it produces. For the last three centuries, the sales of strings alone have been enough to keep business going without a hitch. Now however, the influence of fashion is greater than ever, and you face the prospect of imminent bankruptcy unless you adapt to the needs and fancies of the rather unusual part of society who constitute your main clientele. These elderly ladies have recently decided that fashion has changed: strings are out, and earrings are in. There is nothing to be done about it -- you have to comply and switch to the production of earrings.</p>
<p>
One problem remains: what to do with the impressive heap of amber strings piled up in your shop? One of your assistants has a bright idea: he recommends cutting the strings into two parts, removing some stones to make both parts have an identical color pattern (either immediately, or after rotation by 180 degrees), and selling what remains as pairs of earrings. After a moment's thought, you decide to go ahead with the plan. But your careful managerial eye tells you that minimising the number of wasted (removed) stones may not be as easy as it sounds...</p>
<img src="/content/adrian:jewels.png" alt="Example of string2earring conversion ;)">

<h3>Input</h3>
<p>The first line of input contains a single integer t&lt;=500, the number of test cases. The next t lines contain one test case each, in the form of a string of at most 8000 characters 'a'-'z' (terminated by a new line, optionally preceded by whitespace which should be ignored). The i-th character of the line corresponds to the design on the i-th stone in the amber string it represents. The total length of the input file is not more than 100kB.

</p><h3>Output</h3>
<p>For each test case output two numbers: the largest possible total length of the pair of earrings which can be produced from the string, and a positive integer denoting the number of the stone after which the string ought to be cut so as to achieve this. If more than one cutting position is possible, output the leftmost (smallest) one.

</p><h3>Example</h3>
<pre><b>Input:</b>
3
abcacdd
acbddabedff
abcbca

<b>Output:</b>
4 3
6 4
4 2
</pre>
<p>
(the first case is illustrated in the figure, in the second case we produce a pair of earrings of the form 'abd', in the third - a pair of earrings which look like 'ab' after rotating the second one by 180 degrees).
</p>