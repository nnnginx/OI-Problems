<p>Somewhere deep in the Czech Technical University buildings, there are laboratories for examin-
ing mechanical and electrical properties of various materials. In one of yesterday's presentations,
you have seen how was one of the laboratories changed into a new multimedia lab. But there
are still others, serving to their original purposes.

</p><p>In this task, you are to write software for a robot that handles samples in such a laboratory.
Imagine there are material samples lined up on a running belt. The samples have different
heights, which may cause troubles to the next processing unit. To eliminate such troubles, we
need to sort the samples by their height into the ascending order.

</p><p>Reordering is done by a mechanical robot arm, which is able to pick up any number of consecutive
samples and turn them round, such that their mutual order is reversed. In other words, one
robot operation can reverse the order of samples on positions between A and B.

</p><p>A possible way to sort the samples is to find the position of the smallest one (P_1) and reverse
the order between positions 1 and P_1, which causes the smallest sample to become first. Then
we find the second one on position P_2 and reverse the order between 2 and P_2. Then the third
sample is located etc.

</p><p></p><center><img src="/content/carl:cerc07s.jpg" alt="example"></center>

<p>The picture shows a simple example of 6 samples. The smallest one is on the 4th position,
therefore, the robot arm reverses the first 4 samples. The second smallest sample is the last one,
so the next robot operation will reverse the order of five samples on positions 2-6. The third
step will be to reverse the samples 3-4, etc.

</p><p>Your task is to find the correct sequence of reversal operations that will sort the samples using the above algorithm. If there are more samples with the same height, their mutual order must
be preserved: the one that was given first in the initial order must be placed before the others
in the final order too.


</p><h3>Input</h3>
<p>The input consists of several scenarios. Each scenario is described by two lines. The first line
contains one integer number N, the number of samples, 1 &lt;= N &lt;= 100 000. The second line lists
exactly N space-separated positive integers, they specify the heights of individual samples and
their initial order.

</p><p>The last scenario is followed by a line containing zero.


</p><h3>Output</h3>
<p>For each scenario, output one line with exactly N integers P_1,P_2,...P_N, separated by a space.
Each P_i must be an integer (1 &lt;= P_i &lt;= N) giving the position of the i-th sample just before the
i-th reversal operation.

</p><p>Note that if a sample is already on its correct position P_i, you should output the number P_i
anyway, indicating that the "interval between P_i and P_i" (a single sample) should be reversed.

</p><h3>Example</h3>
<pre><b>Input</b>
6
3 4 5 1 6 2
4
3 3 2 1
0

<b>Output</b>
4 6 4 5 6 6
4 2 4 4

</pre>