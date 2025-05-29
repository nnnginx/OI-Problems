<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>You administer a large cluster of computers with hard drives     that use various file system types to store data. You recently     decided to unify the file systems to the same type. That is     quite a challenge since all the drives are currently in use,     all of them are filled with important data to the limits of     their capacities, and you cannot afford to lose any of the     data. Moreover, reformatting a drive to use a new file system     may significantly change the drive¡¯s capacity. To make the     reformat possible, you will have to buy an extra hard drive.     Obviously, you want to save money by minimizing the size of     such extra storage.</p>
<p>You can reformat the drives in any order. Prior to     reformatting a drive, you must move all data from that drive to     one or more other drives, splitting the data if necessary.     After a drive is reformatted, you can immediately start using     it to store data from other drives. It is not necessary to put     all the data on the same drives they originally started on ¨C in     fact, this might even be impossible if some of the drives have     smaller capacity with the new file system. It is also allowed     for some data to end up on the extra drive.</p>
<p>As an example, suppose you have four drives      $A$,      $B$,      $C$, and      $D$ with drive capacities      $6$,      $1$,      $3$, and      $3$ GB. Under the new file system, the     capacities become $6$,     $7$,      $5$, and      $5$&nbsp;GB, respectively. If you buy     only $1$ GB of extra     space, you can move the data from drive      $B$ there and then reformat drive     $B$. Now you have     $7$ GB free on drive     $B$, so you can move the     $6$ GB from drive     $A$ there and reformat     drive $A$. Finally, you     move the six total gigabytes from drives      $C$ and      $D$ to drive      $A$, and reformat      $C$ and      $D$.</p>
<h3>Input</h3>
<p>Multiple test cases, please process until EOF is reached. For each test case:</p>
<p>The input begins with a line containing one integer     $n$ (     $1 \le n \le 10^6$), which is the     number of drives in your cluster. Following this are     $n$ lines, each describing     a drive as two integers      $a$ and      $b$, where      $a$ is the capacity with the old file     system and $b$ is the     capacity with the new file system.</p>
<p>All capacities are given in gigabytes and satisfy     $1 \le a,b \le 10^9$. (One     thousand petabytes should be enough for everyone, right?)</p>
<h3>Output</h3>
<p>For each test case, display the total extra capacity in gigabytes you must buy     to reformat the drives.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
4
6 6
1 7
3 5
3 5
4
2 2
3 3
5 1
5 10

<strong>Output:</strong>
1
5

</pre>