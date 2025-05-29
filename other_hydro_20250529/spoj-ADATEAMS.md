<p>Ada the Ladybug is a well known mathematician. Next week she is going to represent her school in Mathematic Olympiad. There are many schools participating and each of them has many students. Anyway only some of the students and only some of the schools will be availible to participate in the Olympiad. Question is, how many combinations of students can participate in the Olympiad?</p>
<p>More specifically: There are <strong>N</strong> schools from which exactly <strong>A</strong> will participate. Moreover there are <strong>B</strong> students in each school and exactly <strong>D</strong> of them will participate in the Olympiad.</p>
<p>Ada could count it herself. But this process takes too much time and the limits for schools and students are changing every moment so she has decided to make a program for it (in fact she has decided that you will make the program for her)!</p>
<h3>Input</h3>
<p>The input contains up to <strong>10<sup>4</sup></strong> lines, each containing four integers <strong>N,A,B,D</strong>, <strong>1 ¡Ü A ¡Ü N ¡Ü 10<sup>6</sup></strong>,<strong>1 ¡Ü D ¡Ü B ¡Ü 10<sup>6</sup></strong></p>
<h3>Output</h3>
<p>For each line print the number of combination of students, which can participate in the Olympiad. All students and universities are distinguishable, but their order doesn't matter.</p>
<p>Since the anwer might be huge, print it modulo <strong>10<sup>9</sup>+7</strong> (<strong>1000000007</strong>)</p>
<h3>Example Input</h3>
<pre>2 1 2 2
2 2 2 1
2 1 2 1
4 3 3 2
4 2 1 1
10 4 12 7
50 30 44 20
</pre>
<h3>Example Output</h3>
<pre>2
4
4
108
6
625817778
154746653
</pre>