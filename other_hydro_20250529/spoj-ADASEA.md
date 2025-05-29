<p>Ada the Ladybug just read a book from famous author Dobsonfly Daffoedil. It is about Robinson's Cicada, who was flying over sea. Suddenly she had an accident and fell to island below her. Luckily the island was big enough, so she could recover and fly home till Friday night... or something like that.</p>
<p>As Ada was reading through the book, she fell asleep and started dreaming. She was thinking about how lucky the Cicada was, that she fell into such big island. She could have fallen into a smaller one or even to sea.</p>
<p>It keeps bugging her, so she has asked you to tell her the <a href="https://en.wikipedia.org/wiki/Expected_value">expected size</a> of island, the Cicada will fall to (considering equal probability for all coordinates). Since Ada is not friend of floating point numbers, she wants the answer in some "nice" form.</p>
<p>Island is considered to be union of any '#' characters, which share side.</p>
<h3>Input</h3>
<p>The first line contains an integer <strong>T</strong>, the number of test-cases.</p>
<p>Each test-case begins with two integers <strong>N, M</strong>, <strong>1 ¡Ü N, M ¡Ü 1000 </strong></p>
<p>Afterward <strong>N</strong> lines follow, with <strong>M</strong> characters. Each of the characters is either '<strong>#</strong>' (island) or '<strong>~</strong>' (sea).</p>
<h3>Output</h3>
<p>For each test-case print the expected size of island. Output it as <strong>p / q</strong>, where <strong>p</strong> and <strong>q</strong> has no common divisor. If <strong>p / q</strong> can be printed as an integer (not as fraction), do so!</p>
<h3>Example Input</h3>
<pre>5
3 4
~~~~
~~~~
~~~~
3 3
#~~
##~
~~~
4 5
#~##~
#~~~#
~~~~#
####~
1 1
#
4 4
~~~~
##~~
~##~
##~~
</pre>
<h3>Example Output</h3>
<pre>0
1
7 / 5
1
9 / 4
</pre>