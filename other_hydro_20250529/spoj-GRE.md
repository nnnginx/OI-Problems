<div style="text-align: left; margin: 10px 0px;"><div style="float: right; margin: 0px 0px 3px 10px;"><img src="/content/crazyb0y:GRE.jpg" width="250"></div><span>

<p>Recently George is preparing for the Graduate Record Examinations (GRE for short). Obviously the most important thing is reciting the words.</p>

<p>Now George is working on a word list containing <b>N</b> words. He has so poor a memory that it is too hard for him to remember all of the words on the list. But he does find a way to help him to remember. He finds that if a sequence of words has a property that for all pairs of neighboring words, the previous one is a substring of the next one, then the sequence of words is easy to remember. </p>

<p>So he decides to eliminate some words from the word list first to make the list easier for him. Meantime, he doesn't want to miss the important words. He gives each word an importance, which is represented by an integer ranging from -1000 to 1000, then he wants to know which words to eliminate to maximize the sum of the importance of remaining words. Negative importance just means that George thought it useless and is a waste of time to recite the word. </p>

<p>Note that although he can eliminate any number of words from the word list, he can never change the order between words. In another word, the order of words appeared on the word list is consistent with the order in the input. In addition, a word may have different meanings, so it can appear on the list more than once, and it may have different importance in each occurrence.</p>

</span></div>

<h3>Input</h3>
<p>The first line contains an integer <b>T</b> (1 �� <b>T</b> �� 50), indicating the number of test cases. </p>

<p>Each test case contains several lines.
The first line contains an integer <b>N</b> (1 �� <b>N</b> �� 2��10<sup>4</sup>), indicating the number of words.</p>

<p>Then <b>N</b> lines follows, each contains a string <b>S</b><sub>i</sub> and an integer <b>W</b><sub>i</sub>, representing the word and its importance. <b>S</b><sub>i</sub> contains only lowercase letters.</p>

<p>You can assume that the total length of all words will not exceeded 3��10<sup>5</sup>.</p>

<h3>Output</h3>
<p>For each test case in the input, print one line: <tt>"Case #X: Y"</tt>, where <b>X</b> is the test case number (starting with 1) and <b>Y</b> is the largest importance of the remaining sequence of words.</p>

<h3>Example</h3>

<pre><b>Input:</b>
1
5
a 1
ab 2
abb 3
baba 5
abbab 8

<b>Output:</b>
Case #1: 14
</pre>

<i>There was a serious and subtle problem regarding the test cases. It has been fixed and all submissions were rejudged now.</i>