<p>
<img src="./21609/file/uztGtXfN.png">
</p>
<p>
No wonder the old bookcase caved under the massive piles of books Tom
had stacked on it. He had better build a new one, this time large
enough to hold all of his books. Tom finds it practical to have the
books close at hand when he works at his desk. Therefore, he is
imagining a compact solution with the bookcase standing on the back
of the desk.  Obviously, this would put some restrictions on the size
of the bookcase, it should preferably be as small as possible.  In
addition, Tom would like the bookcase to have exactly three shelves for
aesthetical reasons.
</p>
<p>
Wondering how small his bookcase could be, he models the problem as
follows. He measures the height <em>h<sub>i</sub></em> and thickness
<em>t<sub>i</sub></em> of each book <em>i</em> and he seeks a
partition of the books in three non-empty sets <em>S<sub>1</sub></em>,

<em>S<sub>2</sub></em>, <em>S<sub>3</sub></em> such that
</p>
<p>
<img class="figure" src="./21609/file/ooLQ9p3y.png">
</p>
<p>
is minimized, i.e. the area of the bookcase as seen when standing in
front of it (the depth needed is obviously the largest width of all
his books, regardless of the partition).  Note that this formula does
not give the exact area of the bookcase, since the actual shelves
cause a small additional height, and the sides cause a small
additional width.  For simplicity, we will ignore this small
discrepancy.
</p>
<p>
Thinking a moment on the problem, Tom realizes he will need a computer
program to do the job.
</p>
<h3>Input</h3>
<p>
The input begins with a positive number on a line of its own telling
the number of test cases (at most 20).  For each test case there is
one line containing a single positive integer <em>N</em>, 3 ¡Ü
<em>N</em> ¡Ü 70 giving the number of books. Then <em>N</em> lines
follow each containing two positive integers <em>h<sub>i</sub></em>,
<em>t<sub>i</sub></em>, satisfying 150 ¡Ü <em>h<sub>i</sub></em>

¡Ü 300 and 5 ¡Ü <em>t<sub>i</sub></em> ¡Ü 30, the height and
thickness of book <em>i</em> respectively, in millimeters.
</p>
<h3>Output</h3>
<p>
For each test case, output one line containing the minimum area
(height times width) of a three-shelf bookcase capable of holding all
the books, expressed in square millimeters.
</p>
<h3>Example</h3>

<pre><b>Input:</b>
2
4
220 29
195 20
200 9
180 30
6
256 20
255 30
254 15
253 20
252 15
251 9

<b>Output:</b>
18000
29796
</pre>