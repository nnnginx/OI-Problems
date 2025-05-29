<p>An acronym is made of up the initial letter(s) of the words in a phrase, such as EU (European Union) and BREXIT (BRitish EXIT). In this problem, we can also either ignore or consider the conjunction "<strong>and</strong>", and the following adpositions "<strong>in</strong>", "<strong>on</strong>", "<strong>at</strong>", "<strong>to</strong>", "<strong>of</strong>", "<strong>from</strong>", "<strong>for</strong>" and "<strong>with</strong>" when making the acronym, such as BENELUX (BElgium, NEtherlands and LUXembourg) and RADAR (RAdio Detection And Ranging).</p>
<p>Given an acronym <strong>A</strong>, and a list of <strong>N</strong> strings <strong>W<sub>1</sub></strong>, <strong>W<sub>2</sub></strong> ... <strong>W<sub>N</sub></strong>, you would like to find out the number of possible combinations of making the given acronym by using all the N strings following their order. That is, the acronym must be made up of at least one initial letter of each word, except the above-mentioned conjunction and adpositions (either skip or use it). Both A and the N strings only consist of lowercase latin letters.</p>
<h3>Input</h3>
<p>The first line is the number of test cases <strong>T</strong>. (1&nbsp;¡Ü T ¡Ü 20)</p>
<p>For each test case, it starts with one integer <strong>N</strong>. (1 ¡Ü N ¡Ü 200)</p>
<p>Next line is a string <strong>A</strong>.&nbsp;(1 ¡Ü |A| ¡Ü 10<sup>4</sup>)</p>
<p>Following N lines, each consisting of one string <strong>W<sub>i</sub></strong>. (1 ¡Ü |W<sub>i</sub>| ¡Ü 50)</p>
<p>It is guaranteed that W<sub>1</sub> is neither conjunction nor adposition.</p>
<h3>Output</h3>
<p>Output one integer indicating the number of possible combinations.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3
3
duckhim
duck
hello
moto

7
natiofforessaa
national
office
for
forest
safety
in
aachen

4
whiskey
what
is
secret
key

<strong>Output:</strong>
0
4
1
</pre>
<h3>Explanation</h3>
<p>In case 1, no combination is possible.</p>
<p>In case 2, there are four possible combinations:</p>
<ul>
<li><strong>NATI</strong>onal <strong>OF</strong>fice for <strong>FORES</strong>t <strong>SA</strong>fety in <strong>A</strong>achen</li>
<li><strong>NATI</strong>onal <strong>OF</strong>fice for <strong>FORES</strong>t <strong>S</strong>afety in <strong>AA</strong>chen</li>
<li><strong>NATI</strong>onal <strong>O</strong>ffice <strong>F</strong>or <strong>FORES</strong>t <strong>SA</strong>fety in <strong>A</strong>achen</li>
<li><strong>NATI</strong>onal <strong>O</strong>ffice <strong>F</strong>or <strong>FORES</strong>t <strong>S</strong>afety in <strong>AA</strong>chen</li>
</ul>
<p>In case 3, only one possible combination exists:</p>
<ul>
<li><strong>WH</strong>at <strong>I</strong>s <strong>S</strong>ecret <strong>KEY</strong></li>
</ul>