<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Here we go!</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Let's define the diversity of a list of numbers to be the difference between the largest and smallest number in the list.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">For example, the diversity of the list (1, -1, 2, 7) = 7 - (-1) = 8.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">A substring of a list is considered a non-empty sequence of contiguous numbers from the list. For example, for the list (1,3,7), the substrings are (1), (3), (7), (1,3), (3,7), (1,3,7). A subsequence of a list is defined to be a non-empty sequence of numbers obtained by deleting some elements from the list. For example, for the list (1,3,7), the subsequences are (1), (3), (7), (1,3), (3,7), (1,7), (1,3,7).</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Given a list of length N find the number of substrings and subsequences in this list with the maximum diversity. If a substring/subsequence having maximum diversity occurs multiple times in the list, each of its occurances adds towards the answer. &nbsp; And tell Harry Potter your answer.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Input (STDIN):</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The first line contains T, the number of test cases. Then follow T test case blocks.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Each blocks starts with the first line containing the number N.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The second line contains a list of numbers in this list.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Output (STDOUT):</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">For each test case, output the number of substrings and the number of subsequences in this list with the maximum diversity.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Since the answers maybe very large, output them modulo 1000000007.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Constraints:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">T &lt;= 10</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">N &lt;= 100,000</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Each number in the list is between 1 and 100,000 inclusive.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Time Limit: 2 s</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Memory Limit: 32 MB</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Sample Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1 2 3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">4</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1 4 3 4</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">3 2 1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Sample Output:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1 2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">3 6</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">12</div>
<p>Enough with this Harry Potter, please! What are we, twelve-year olds? &nbsp;Let's get our teeth into some real pumpkin pasties -- oops, programming problems!</p>
<p>&nbsp;</p>
<p>Here we go!</p>
<p>Let's define the diversity of a list of numbers to be the difference between the largest and smallest number in the list.</p>
<p>For example, the diversity of the list (1, -1, 2, 7) = 7 - (-1) = 8.</p>
<p>&nbsp;</p>
<p>A substring of a list is considered a non-empty sequence of contiguous numbers from the list. For example, for the list (1,3,7), the substrings are (1), (3), (7), (1,3), (3,7), (1,3,7). A subsequence of a list is defined to be a non-empty sequence of numbers obtained by deleting some elements from the list. For example, for the list (1,3,7), the subsequences are (1), (3), (7), (1,3), (3,7), (1,7), (1,3,7).</p>
<p>&nbsp;</p>
<p>Given a list of length N find the number of substrings and subsequences in this list with the maximum diversity. If a substring/subsequence having maximum diversity occurs multiple times in the list, each of its occurences adds towards the answer. &nbsp; And tell Harry Potter your answer</p>
<p>&nbsp;</p>
<p><strong>Input (STDIN):</strong></p>
<p>The first line contains T, the number of test cases. Then follow T test case blocks.</p>
<p>Each blocks starts with the first line containing the number N.</p>
<p>The second line contains a list of numbers in this list.</p>
<p>&nbsp;</p>
<p><strong>Output (STDOUT):</strong></p>
<p>For each test case, output the number of substrings and the number of subsequences in this list with the maximum diversity.</p>
<p>Since the answers maybe very large, output them modulo 1000000007.</p>
<p>&nbsp;</p>
<p><strong>Constraints:</strong></p>
<p>T &lt;= 10</p>
<p>N &lt;= 100,000</p>
<p>Each number in the list is between 1 and 100,000 inclusive.</p>
<p>&nbsp;</p>
<p><strong>Sample Input:</strong></p>
<p>3</p>
<p>3</p>
<p>1 2 3</p>
<p>4</p>
<p>1 4 3 4</p>
<p>3</p>
<p>3 2 1</p>
<p>&nbsp;</p>
<p><strong>Sample Output:</strong></p>
<p>&nbsp;</p>
<p>1 2</p>
<p>3 6</p>
<p>1 2</p>
<p>&nbsp;</p>
<p>&nbsp;</p>