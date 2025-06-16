<p><span style="font-family: 'Times New Roman'; font-size: 16px;">California Jones (the sister of famous Indiana Jones) once again faced a seemingly intractable problem. Her only hope was in you. She knew you were a computer scientist and you might have a clue.</span></p>
<p style="font-family: Times, serif; text-align: justify; font-size: 16px;">Jones calls you on the video-phone and tells you the facts: she walked into a trap and now stands in front of a huge gate. On the left side strange signs can be seen while&nbsp;<em>n</em>&nbsp;stones lie on the right side. In front of the gate there are exactly&nbsp;<em>n/2</em>&nbsp;holes. Says Jones, "I suppose I have to take exactly half of the stones from the right side and put them into the holes." Ancient writings confirm her conjecture. According to the writings it does not matter which hole a stone is placed into. It is only important that the right stones are chosen.</p>
<table style="margin: auto; width: 100%;" border="0" cellpadding="0">
<tbody>
<tr>
<td valign="TOP"><img style="display: block; margin: auto;" src="./24844/file/HFvmg97J.png" alt=""></td>
<td valign="TOP">
<table style="margin: auto;" border="0">
<tbody>
<tr>
<td>Nearby, Jones found a stone board, too, but was unable to interpret. It made sense to you though. It was a hint on how to sort the various possibilities of chosing&nbsp;<em>n/2</em>&nbsp;stones.
<p style="font-family: Times, serif; text-align: justify;">But you couldn't yet figure out about the zeros and the ones. So you asked Jones who replied that "the same symbols I saw on the left side of the gate - only they were somewhat longer sequences. But I haven't met such a primitive civilization yet."</p>
<p style="font-family: Times, serif; text-align: justify;">Now everything was clear to you: the symbols were the representation of a binary number - and it indicated which stones to choose. Simply ingenious! Jones was enthusiastic about you.</p>
<p style="font-family: Times, serif; text-align: justify;">But it was impossible for Jones to calculate for a given binary number the corresponding stones. So she instructed you to write a program to solve the task and help her through the gate to freedom. Five hours later, she would call back.</p>
<p style="font-family: Times, serif; text-align: justify;">Take a thorough look at the figure to the left depicting the stone board, as well as the sample input and output, to figure out how to solve Jones' problem.</p>
</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>
<p style="font-family: Times, serif; text-align: justify; font-size: 16px;"><strong>Input Specification</strong></p>
<p style="font-family: Times, serif; text-align: justify; font-size: 16px;">The input contains several testcases. Each starts with the number of stones&nbsp;<em>n</em>. Input is terminated by&nbsp;<em>n=0</em>. Otherwise,&nbsp;<em>n</em>&nbsp;is even and&nbsp;<em>2��n��32</em>. The next&nbsp;<em>n</em>&nbsp;integers identify the stones. A test case is further subdivided into&nbsp;<em>k</em>&nbsp;(sub-) test cases,&nbsp;<em>k</em>&nbsp;being the next number in the input file. Then follow&nbsp;<em>k</em>&nbsp;times a bit string&nbsp;<em>b</em>&nbsp;(encoding a non-negative integer) and&nbsp;<em>n/2</em>&nbsp;distinct integers identifying the set of chosen stones. No invalid stones will be chosen and the length of&nbsp;<em>b</em>&nbsp;will not exceed&nbsp;<em>30</em>.</p>
<p style="font-family: Times, serif; text-align: justify; font-size: 16px;"><strong>Output Specification</strong></p>
<p style="font-family: Times, serif; text-align: justify; font-size: 16px;">For each (sub-) test case generate a line containing&nbsp;<tt>TRUE</tt>, if the chosen stones may be laid into the holes, and&nbsp;<tt>FALSE</tt>&nbsp;otherwise.</p>
<p style="font-family: Times, serif; text-align: justify; font-size: 16px;"><strong>Sample Input</strong></p>
<p style="font-family: Times, serif; text-align: justify; font-size: 16px;"><tt></tt></p>
<pre style="font-size: 16px;"><tt>4
12 50 74 34
1
00
50 12

8
45 23 86 43 90 76 12 74
2
111001
86 43 90 74
010001
45 86 43 90

4
12 50 74 34
2
101
34 74
110
34 74

0
</tt></pre>
<p style="font-family: Times, serif; text-align: justify; font-size: 16px;"><strong>Sample Output</strong></p>
<p style="font-family: Times, serif; text-align: justify; font-size: 16px;"><tt></tt></p>
<pre style="font-size: 16px;"><tt>TRUE
TRUE
FALSE
TRUE
FALSE
</tt></pre>
<div><tt><br></tt></div>