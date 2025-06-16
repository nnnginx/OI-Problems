<p>Ada the Ladybug is already planning her birthday party. It is not an easy process since she have many friends but each of her friends likes just about half of her other friends. She wants to invite only such subset of friends that everyone likes each other.</p>
<p>Ada has barely some time and she wants big party so she asked you to find maximum such list in which each of her friends is friend with each of her other friends on the list.</p>
<h3>Input</h3>
<p>The first line contains an integer <strong> 1 ¡Ü T ¡Ü 100</strong>, the number of test-cases.</p>
<p>The first line of each test-case begins with <strong>1 ¡Ü N ¡Ü 130</strong>, the number of her friends.</p>
<p>Each of next <strong>N</strong> lines contain <strong>N</strong> integers <strong>A<sub>i,j</sub></strong> (either <strong>0</strong> or <strong>1</strong>), where <strong>1</strong> means the <strong>i<sup>th</sup></strong> friend likes <strong>j<sup>th</sup></strong> (and <strong>0</strong> means the opposite)</p>
<p>Important note is, that as brain connections of insect are not so complicated as those of humans, so the process of making friends is slightly different. Two insects have exactly 50% chance of being friends, so also the adjancecy matrix will be generated (very)pseudo-randomly with 50% chance for each edge.</p>
<p>Also note, that the matrix will be symmetrical.</p>
<p>Each insect is friend with itself!</p>
<h3>Output</h3>
<p>For each test-case output the maximum number of Ada's friends, which can be invited.</p>
<h3>Example Input</h3>
<pre>10
7
1 1 0 0 1 1 0
1 1 1 0 1 1 0
0 1 1 0 1 0 1
0 0 0 1 0 0 1
1 1 1 0 1 1 0
1 1 0 0 1 1 0
0 0 1 1 0 0 1
5
1 1 1 1 0
1 1 1 0 1
1 1 1 1 0
1 0 1 1 0
0 1 0 0 1
1
1
4
1 0 0 1
0 1 0 1
0 0 1 0
1 1 0 1
1
1
10
1 1 0 1 0 1 0 1 1 1
1 1 0 1 0 0 1 0 0 0
0 0 1 0 0 0 0 0 1 0
1 1 0 1 1 1 1 0 1 0
0 0 0 1 1 0 0 0 1 1
1 0 0 1 0 1 0 1 0 0
0 1 0 1 0 0 1 0 1 1
1 0 0 0 0 1 0 1 1 1
1 0 1 1 1 0 1 1 1 0
1 0 0 0 1 0 1 1 0 1
7
1 1 0 1 1 0 0
1 1 1 0 1 0 0
0 1 1 0 0 1 0
1 0 0 1 1 0 0
1 1 0 1 1 0 1
0 0 1 0 0 1 0
0 0 0 0 1 0 1
3
1 1 0
1 1 1
0 1 1
8
1 0 1 1 1 1 0 0
0 1 0 1 1 1 1 1
1 0 1 1 0 1 0 1
1 1 1 1 1 0 1 1
1 1 0 1 1 1 0 1
1 1 1 0 1 1 1 1
0 1 0 1 0 1 1 1
0 1 1 1 1 1 1 1
6
1 0 1 0 0 1
0 1 0 0 0 1
1 0 1 1 1 0
0 0 1 1 0 1
0 0 1 0 1 0
1 1 0 1 0 1
</pre>
<h3>Example Output</h3>
<pre>4
3
1
2
1
3
3
2
4
2
</pre>