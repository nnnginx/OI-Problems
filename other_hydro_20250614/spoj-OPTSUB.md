<div align="justify">
    <ul>
        <li>
        A point <i>P</i>(<i>x</i>,<i>y</i>) is called an integer point if and only if both <i>x</i> and <i>y</i> are integers.
        </li><li>
        <i>W</i> is the set which contains all the integer points on the plane.
        </li><li>
        Two integer point <i>P</i>(<i>x</i>,<i>y</i>) and <i>Q</i>(<i>x'</i>,<i>y'</i>) are called adjacent if and only if <i>|x-x'|+|y-y'|=1</i>.
        </li><li>
        <i>S</i> is a set of integer points if and only if <i>S</i> is a limited subset of <i>W</i>.
        </li><li>
        If <i>S</i> is a set of integer points, <i>R</i> and <i>T</i> belong to <i>S</i>,and there exist a limited integer point sequence <i>Q</i><sub>0</sub>(=<i>R</i>),<i>Q</i><sub>1</sub>,<i>Q</i><sub>2</sub>,...,<i>Q</i><sub>k</sub>,<i>Q</i><sub>k+1</sub>(=<i>T</i>) which satisfies that
        <div align="justify">
            <ul>
                <li>
                <i>Q</i><sub>i</sub>!=<i>Q</i><sub>j</sub> iff <i>i</i>!=<i>j</i>
                </li><li>
                <i>Q</i><sub>i</sub> and <i>Q</i><sub>i+1</sub> are adjacent, for each 0&lt;=<i>i</i>&lt;=k.
                </li><li>
                <i>Q</i><sub>i</sub> belongs to <i>S</i>, for each 0&lt;=<i>i</i>&lt;=k+1.</li>
            </ul>
        </div>
       we call <i>R</i> and <i>T</i> are connected and the sequence <i>Q</i><sub>i</sub>(0&lt;=i&lt;=k) is a path that connect <i>R</i> and <i>T</i>.
        </li><li>
        If <i>S</i> is a set of integer points, <i>X</i> and <i>Y</i> are some integer points that belong to <i>S</i>, there exists one and only one path connected <i>X</i> and <i>Y</i>, then <i>S</i> is called an optimal set.</li>
    </ul>
</div>
<p>Given an optimal set <i>V</i>, your task is to find an optimal set <i>B</i>, satisfying that <i>B</i> is a subset of <i>V</i> and the sum of the weights of each integer point is maximum.</p>
<h3>Input</h3>
<p>The very first line of the input contains a single integer <i>T</i>, the number of test cases. <i>T</i> blocks follow.</p>
<p>For each test case, the first line contains a single integer <i>N</i>=|<i>V</i>|(<i>N</i>&lt;=1000). <i>N</i> lines follow, each contains 3 integers, the X-coordinate, the Y-coordinate and the weight(the absolute value of the weight&lt;=100) of the <i>i</i>th integer point, separated by single spaces.</p>
<h3>Output</h3>
<p><i>T</i> lines,each contains a single integer - the maximum sum of weights.</p>
<h3>Example</h3>
<pre><b>Input:</b>
1
5
0 0 -2
0 1 1
1 0 1
0 -1 1
-1 0 1

<b>Output:</b>
2
</pre>