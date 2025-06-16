<p>Little Petar and his fellow hacker Little Nikolaj enjoy playing the "SIGSEGV" game against one another in their free time, as all hackers do. In this game, two hackers compete for supremacy over a victim's RAM. To achieve this, they need to develop programs that will capture as many memory locations as possible for their own.</p>
<p>The rules of the game are as follows:</p>
<ul>
<li>The RAM is represented by a matrix, RAM[][]; each field of this matrix may either be <strong>free</strong>, owned by Petar or Nikolaj, or owned by the <strong>victim</strong>.</li>
<li>Petar and Nikolaj's programs begin execution from a field of this matrix, and are able to perform only a single type of command: "move to the field directly up, down, left or right from the current field, and attempt capturing it."</li>
<li>If a program tries to capture a field that is not free and also not owned by its owner, it will receive a <strong>segfault</strong> (<em>segmentation fault</em>) signal and <strong>terminate immediately</strong>; however, the hacker owning it will <strong>retain</strong> all the memory that the program captured.</li>
<li>Petar and Nikolaj may launch <strong>many</strong> programs <strong>simultaneously</strong>, should they have access to a multi-core computer. The programs may be launched <strong>only</strong> at the <strong>start</strong> of the game.</li>
</ul>
<p>Each hacker has gained an unfair advantage over the other:</p>
<ul>
<li>Nikolaj managed to make his capturing scheme faster, so if Petar and Nikolaj both attempt to capture the same (free) field at the same time, Nikolaj's program will capture it and Petar's program will terminate.</li>
<li>Nikolaj owns a K-core computer, so he may launch K programs at the start of the game.</li>
<li>Petar found out the entire initial state of the memory, as well as all of Nikolaj's programs. As Nikolaj doesn't know the initial state, he programmed his programs to be very simple: they begin at a given field and will always move in a single given direction (until encountering either the end of the matrix or a non-free field not owned by Nikolaj, after which it terminates).</li>
<li>Nikolaj's programs will start their execution only after Petar's programs capture the initial field.</li>
<li>Due to a virus that Nikolaj inserted in Petar's programs, all of them must start from the same field.</li>
<li>Petar owns the latest Pintel Core i�� processor that has infinitely many cores; as such, Petar may initially launch an arbitrary number of programs (however, they must all start from the same field, as mentioned before).</li>
</ul>
<ul>
</ul>
<ul>
</ul>
<p>Petar is interested in knowing how many fields of the RAM can he capture if he plays optimally.</p>
<h3>Input</h3>
<p>The first line of the standard input contains two natural numbers N and M separated by a space; these represent the number of rows and columns of the RAM[][] matrix, respectively.</p>
<p>The following N lines contain an M-character string each, representing the initial state of the memory (RAM[i][j] is represented by the j-th character in the i-th line):</p>
<ul>
<li>Character '.' represents a free field;</li>
<li>Character '#' represents a field owned by the victim;</li>
<li>Character 'S' represents the field from which all of Petar's programs must start.</li>
</ul>
<p>The following line contains a natural number K, the number of cores of Nikolaj's processor. Each of the following K lines contains the description of one of Nikolaj's programs, in the form X Y DIR, where X and Y are integers representing the program's starting field, and DIR is a character representing the program's only direction of movement ('U' - up, 'D' - down, 'L' - left, 'R' - right).</p>
<h3>Output</h3>
<p>In the first and only line of the standard output, print the number of memory locations that Petar may capture, assuming he plays optimally.</p>
<h3>Example</h3>
<pre><strong>Input:<br></strong>6 5<br>#.S.#<br>.....<br>.....<br>...##<br>##...<br>...##<br>2<br>2 1 R<br>3 5 L</pre>
<pre><strong>Output:</strong>
18</pre>
<h3>Explanation</h3>
<p>Petar can achieve the optimal strategy with only launching a single program; this program should make its first two steps downwards, and the state of the RAM will change as follows (let 'P' represent fields owned by Petar, and 'N' represent the fields owned by Nikolaj):</p>
<div title="Page 2">
<div>
<div>
<p><span style="font-size: 11.000000pt; font-family: 'Courier';">#.P.# &nbsp; &nbsp;#.P.# &nbsp; &nbsp;#.P.# </span></p>
<p><span style="font-size: 11.000000pt; font-family: 'Courier';">..... &nbsp; &nbsp;N.P.. &nbsp; &nbsp;NNP.. </span></p>
<p><span style="font-size: 11.000000pt; font-family: 'Courier';">..... =&gt; ....N =&gt; ..PNN </span></p>
<p><span style="font-size: 11.000000pt; font-family: 'Courier';">...## =&gt; ...## =&gt; ...## </span></p>
<p><span style="font-size: 11.000000pt; font-family: 'Courier';">##... &nbsp; &nbsp;##... &nbsp; &nbsp;##... </span></p>
<p><span style="font-size: 11.000000pt; font-family: 'Courier';">...## &nbsp; &nbsp;</span><span style="font-family: Courier; font-size: 11pt;">...## &nbsp; &nbsp;...##</span></p>
<ul>
</ul>
<p>Both of Nikolaj's programs will hence receive a segfault in the next step, leaving Petar free to capture all of the remaining fields of the matrix (18 in total).</p>
<h3>Constraints</h3>
<ul>
<li>1 &lt;= N, M &lt;= 1000</li>
<li>1 &lt;= K &lt;= 5 * 10<sup>5</sup></li>
<li>1 &lt;= X &lt;= N</li>
<li>1 &lt;= Y &lt;= M</li>
<li>RAM[X][Y] is not equal to '#'.</li>
</ul>
</div>
</div>
</div>