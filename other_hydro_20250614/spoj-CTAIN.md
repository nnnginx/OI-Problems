<p>
   </p><p>We are given <i>n</i> containers, where 1 &lt;= <i>n</i> &lt;= 4. At
        the beginning all of them are full of water. The liter capacity of the <i>i</i>-th
        container is a natural number <i>o</i><sub><i>i</i> </sub>satisfying
        inequalities 1 &lt;= <i>o<sub>i</sub> </i>&lt;= 49.&nbsp;<br>
        Three kinds of moves can be made: &nbsp;
        </p><ol type="1">
          <li>Pouring the whole content of one container into another. This move
            can be made unless there is too little room in the second container.&nbsp;
          </li><li>Filling up one container with part of the water from another one.
          </li><li>Pouring away the whole content of one container into a drain.&nbsp;<br>
          </li>
        </ol>
<p></p>
<h3>Task</h3>
<p>
  </p><p>Write a program that for each test case:</p>
        <ul type="disc">
          <li>Reads the number of containers <i>n</i>, the capacity of each container and the requested final amount of water in each container.
          </li><li>Verifies, whether there exist a series of moves which leads to the        requested final situation, and if there is one, the program computes the minimal number of moves leading to the requested situation,  </li><li>Writes the result. The result should be the minimal number of moves leading to the requested final situation, or one word "NO" if there is no such a sequence of moves.</li>
        </ul>
<p></p>

<h3>Input</h3>
<p>One integer in the first line, stating the number of test cases, followed by a blank line. There will be not more than 20 tests.</p>
<p>For each test case, at the first line, one positive integer <i>n</i>
        is written, <i>n</i> &lt;= 4, this is the number of containers. There
        are <i>n</i> positive integers written in the second line. These are the
        capacities of the containers (the <i>i</i>-th integer <i>o</i><sub><i>i</i></sub>
        denotes the capacity if the <i>i</i>-th&nbsp; container,1 &lt;= <i>o</i><sub><i>i</i></sub>
        &lt;= 49). In the third line there are written <i>n</i>
        numbers. These are the requested final volumes of water in the
        containers (the <i>i</i>-th integer <i>w</i><sub><i>i</i></sub> denotes
        the requested final volume of water in the <i>i</i>-th container, 0
        &lt;= <i>w</i><sub><i>i</i></sub> &lt;= <i>o</i><sub><i>i</i></sub>).
        All integers in the second and the third line are separated by single
        spaces.</p>
<p>The test cases will be separated by a single blank line. </p> 

<h3>Output</h3>
<p>For each test case : write one integer - the minimal number of moves which lead to the requested final situation or write only one word "NO" if it is not possible to reach the requested final situation making only allowed moves.

</p><h3>Example</h3>

<pre><b>Input:</b>
2

3
3 5 5
0 0 4

2
20 25
10 16

<b>Output:</b>
6
NO
</pre>