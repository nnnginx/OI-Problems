<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">'Though the Stewards deemed that it was a secret kept only by themselves, long ago I guessed that here in the White Tower, one at least of the Seven Seeing Stones was preserved. In the days of his wisdom Denethor did not presume to use it, nor to challenge Sauron, knowing the limits of his own strength. But his wisdom failed; and I fear that as the peril of his realm grew he looked in the Stone and was deceived: far too often, I guess, since Boromir departed. He was too great to be subdued to the will of the Dark Power, he saw nonetheless only those things which that Power permitted him to see.' - Gandalf.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Sauron and Saruman have been communicating from large distances using the Seeing Stones. Denethor, with great difficulty has been able to break into their channel of communication using his strength of will. Despite this however, it seems that their communication has been encrypted. Gondor's spies in Isengard have found out the encryption algorithm they use and have reported back to Denethor.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The algorithm is as follows :</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">We refer to a dequeue as a double-ended queue. We define a "dequeue permutation of N" as a permutation of 1 to N that can be got by starting from a dequeue having elements 1, 2, 3, ..., N (in that order with 1 at the front and N at the back) and performing any sequence of N pop_front() or pop_back() operations.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Note that not all permutations of 1 to N are dequeue permutations. For example, with N = 3, you have 3-1-2, 1-3-2 etc. as dequeue permutations whereas 2-1-3, 2-3-1 aren't (you can't have 2 right at the beginning since its not at any end of the dequeue).</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">If Sauron wants to encrypt the number K and send it to Saruman, he would instead send the K'th lexicographically smallest (0-based indexed) dequeue permutation of N. That is, if Sauron wanted to send '0' to Saruman, he would just send 1-2-3-...-N (since this is clearly the smallest lexicographic dequeue permutation of N).</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Sauron is transmitting the size of his army to Saruman, so that they can coordinate an attack on the Men of Rohan and Gondor. Since Sauron's will is so powerful, Denethor is able to get only vague glimpses of the numbers, and he is able to remember only the first half (floor(N/2) elements) of the permutation. Further, since these images are so vague, his understanding of the numbers happens out of order. For example, Denethor may understand that the 5th number of the permutation is 4, and later on only understand that the 3rd number was 3.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Help him estimate the minimum and maximum possible size of Sauron's army (value of K), given the number N, and incremental understanding of the first half of the permutation, not necessarily in order.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">NOTE 1: Since the values to be output can be rather large, output the values modulo 1,000,000,007.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">NOTE 2: It may be the case that Denethor's understanding of the permutation is flawed. If it is not possible to have a dequeue permutation satisfying all the conditions seen so far, output -1.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">NOTE 3: A permutation p1 is lexicographically smaller than p2 if at the first position where they differ, p1's value is smaller than p2's.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Input (STDIN):</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The first line consists of the integer T, the number of test cases.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Each test case begins with a single integer N.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">This is followed by exactly floor(N/2) lines containing 2 integers each: i and j, denoting that Denethor has understood that the i'th element (1-based) of the supposed permutation is j.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Output (STDOUT):</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">For each testcase, output exactly floor(N/2) lines, one for each (i,j) pair. If the recollections till now cannot all be feasible, output '-1' on a line. Else output two space-separated integers: the minimum and the maximum possible value of Sauron's army, K, that are consistent with all the observations seen so far.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Between successive test cases, there should not be any blank lines in the output.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Constraints:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1 &lt;= T &lt; 3&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2 &lt;= N &lt;= 100,000</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1 &lt;= i &lt;= floor(N/2)</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1 &lt;= j &lt;= N</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">All (i, j) pairs are distinct. And for two pairs (i1, j1) and (i2, j2), you have that i1 != i2 and j1 != j2.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Sample Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1 3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">32</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1 1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">3 2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2 32</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">4 4</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">5 5</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">6 6</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">7 7</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">8 8</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">9 9</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">10 10</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">11 11</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">12 12</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">13 13</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">14 14</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">15 15</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">16 3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Sample Output:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2 3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">0 73741816</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">536870912 805306367</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">536870912 805306367</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">-1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">-1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">-1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">-1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">-1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">-1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">-1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">-1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">-1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">-1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">-1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">-1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">-1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Notes/Explanation of Sample Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">For the first test case, for N = 3, there are 4 dequeue permutations, lexicographically ordered as 1-2-3, 1-3-2, 3-1-2, and 3-2-1. Denethor sees the first number of the dequeue permutation as 3, and concludes that the permutation can be either 3-1-2, or 3-2-1.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">In the second test case, we see that</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">(a) the 1st number is 1.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">(b) the 3rd number is 2 ... this means that the 2nd number has to be 32.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">(c) the 2nd number is 32 ... this does not add any new information.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">(d) the 4th number is 4. But this is not possible, since the 4th number can now either be 3 or 31.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Hence it is inconsistent (and none of the further observations can make it consistent).</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Also notice that in the 2nd test-case, the values have been output modulo 1,000,000,007.</div>
<p>'Though the Stewards deemed that it was a secret kept only by themselves, long ago I guessed that here in the White Tower, one at least of the Seven Seeing Stones was preserved. In the days of his wisdom Denethor did not presume to use it, nor to challenge Sauron, knowing the limits of his own strength. But his wisdom failed; and I fear that as the peril of his realm grew he looked in the Stone and was deceived: far too often, I guess, since Boromir departed. He was too great to be subdued to the will of the Dark Power, he saw nonetheless only those things which that Power permitted him to see.' - Gandalf.</p>
<p>Sauron and Saruman have been communicating from large distances using the Seeing Stones. Denethor, with great difficulty has been able to break into their channel of communication using his strength of will. Despite this however, it seems that their communication has been encrypted. Gondor's spies in Isengard have found out the encryption algorithm they use and have reported back to Denethor.</p>
<p>&nbsp;</p>
<p>The algorithm is as follows :</p>
<p>We refer to a dequeue as a double-ended queue. We define a "dequeue permutation of N" as a permutation of 1 to N that can be got by starting from a dequeue having elements 1, 2, 3, ..., N (in that order with 1 at the front and N at the back) and performing any sequence of N pop_front() or pop_back() operations.&nbsp;</p>
<p>Note that not all permutations of 1 to N are dequeue permutations. For example, with N = 3, you have 3-1-2, 1-3-2 etc. as dequeue permutations whereas 2-1-3, 2-3-1 aren't (you can't have 2 right at the beginning since its not at any end of the dequeue).</p>
<p>&nbsp;</p>
<p>If Sauron wants to encrypt the number K and send it to Saruman, he would instead send the K'th lexicographically smallest (0-based indexed) dequeue permutation of N. That is, if Sauron wanted to send '0' to Saruman, he would just send 1-2-3-...-N (since this is clearly the smallest lexicographic dequeue permutation of N).</p>
<p>Sauron is transmitting the size of his army to Saruman, so that they can coordinate an attack on the Men of Rohan and Gondor. Since Sauron's will is so powerful, Denethor is able to get only vague glimpses of the numbers, and he is able to remember only the first half (floor(N/2) elements) of the permutation. Further, since these images are so vague, his understanding of the numbers happens out of order. For example, Denethor may understand that the 5th number of the permutation is 4, and later on only understand that the 3rd number was 3.&nbsp;</p>
<p>&nbsp;</p>
<p>Help him estimate the minimum and maximum possible size of Sauron's army (value of K), given the number N, and incremental understanding of the first half of the permutation, not necessarily in order.</p>
<p>&nbsp;</p>
<p><strong>NOTE 1</strong>: Since the values to be output can be rather large, output the values modulo 1,000,000,007.</p>
<p><strong>NOTE 2</strong>: It may be the case that Denethor's understanding of the permutation is flawed. If it is not possible to have a dequeue permutation satisfying all the conditions seen so far, output -1.</p>
<p><strong>NOTE 3</strong>: A permutation p1 is lexicographically smaller than p2 if at the first position where they differ, p1's value is smaller than p2's.</p>
<p>&nbsp;</p>
<p><strong>Input (STDIN):</strong></p>
<p>The first line consists of the integer T, the number of test cases.</p>
<p>Each test case begins with a single integer N.</p>
<p>This is followed by exactly floor(N/2) lines containing 2 integers each: i and j, denoting that Denethor has understood that the i'th element (1-based) of the supposed permutation is j.</p>
<p>&nbsp;</p>
<p><strong>Output (STDOUT):</strong></p>
<p>For each testcase, output exactly floor(N/2) lines, one for each (i,j) pair. If the recollections till now cannot all be feasible, output '-1' on a line. Else output two space-separated integers: the minimum and the maximum possible value of Sauron's army, K, that are consistent with all the observations seen so far.</p>
<p>Between successive test cases, there should not be any blank lines in the output.</p>
<p>&nbsp;</p>
<p><strong>Constraints:</strong></p>
<p>1 &lt;= T &lt; 3&nbsp;</p>
<p>2 &lt;= N &lt;= 100,000</p>
<p>1 &lt;= i &lt;= floor(N/2)</p>
<p>1 &lt;= j &lt;= N</p>
<p>All (i, j) pairs are distinct. And for two pairs (i1, j1) and (i2, j2), you have that i1 != i2 and j1 != j2.</p>
<p>&nbsp;</p>
<p><strong>Sample Input:</strong></p>
<p>2</p>
<p>3</p>
<p>1 3</p>
<p>32</p>
<p>1 1</p>
<p>3 2</p>
<p>2 32</p>
<p>4 4</p>
<p>5 5</p>
<p>6 6</p>
<p>7 7</p>
<p>8 8</p>
<p>9 9</p>
<p>10 10</p>
<p>11 11</p>
<p>12 12</p>
<p>13 13</p>
<p>14 14</p>
<p>15 15</p>
<p>16 3</p>
<p>&nbsp;</p>
<p><strong>Sample Output:</strong></p>
<p>2 3</p>
<p>0 73741816</p>
<p>536870912 805306367</p>
<p>536870912 805306367</p>
<p>-1</p>
<p>-1</p>
<p>-1</p>
<p>-1</p>
<p>-1</p>
<p>-1</p>
<p>-1</p>
<p>-1</p>
<p>-1</p>
<p>-1</p>
<p>-1</p>
<p>-1</p>
<p>-1</p>
<p>&nbsp;</p>
<p><strong>Notes/Explanation of Sample Input:</strong></p>
<p>For the first test case, for N = 3, there are 4 dequeue permutations, lexicographically ordered as 1-2-3, 1-3-2, 3-1-2, and 3-2-1. Denethor sees the first number of the dequeue permutation as 3, and concludes that the permutation can be either 3-1-2, or 3-2-1.</p>
<p>In the second test case, we see that</p>
<p>(a) the 1st number is 1.</p>
<p>(b) the 3rd number is 2 ... this means that the 2nd number has to be 32.</p>
<p>(c) the 2nd number is 32 ... this does not add any new information.</p>
<p>(d) the 4th number is 4. But this is not possible, since the 4th number can now either be 3 or 31.&nbsp;</p>
<p>Hence it is inconsistent (and none of the further observations can make it consistent).</p>
<p>Also notice that in the 2nd test-case, the values have been output modulo 1,000,000,007.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>