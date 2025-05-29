<p>Given a system of linear equations, print the solution of that system.</p>
<h3>Input</h3>
<p>Input starts with a positive integer t&lt;100 in a single line, then t testcases follow. Every testcase represents a linear system and starts with one line containing a positive integer n&lt;21, the number of equations and also the number  of variables of that system. Then n equations follow, each one in a single line. <br> An equation is written in schoolbook notation, i.e. variables noted by single small letters (english alphabet), no multiplication sign, factor 1 left out, no spaces in between.  A variable or a value may occur zero or more times in an equation. All coefficients are integers with an absolute value less than 100, a single line won't be longer than 100 characters and will always contain a valid linear equation.</p>
<p>The following equations are considered to be <span style="font-weight:bold; color:green">valid</span>:<br> a+b-c+b-2c-a=1 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; -x+5-9=-4x+y-8 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; c-c+t+1=0 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; y=z</p>
<p>The following equations are considered to be <span style="font-weight:bold; color:red">invalid</span>:<br> 4*a+b=6 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 6+-2x=99 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; c-c+t-t=0 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 4+9 = h</p>
<h3>Output</h3>
<p>For each testcase print all variables of the linear system in alphabetical order together with the associated value  as an integer or a fraction in lowest terms respectively. Print a blank line between testcases.  For exact notation see example below. All (interim) results will fit into 64-bit,  if algorithm is implemented properly. You can assume that all linear systems have an unique solution.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
2
a+b=5
b-a=1
3
5u-5z+4=0
8k-3z=-2
9k-u=u
 
<strong>Output:</strong>
a=2
b=3

k=-4/55
u=-18/55
z=26/55
</pre>