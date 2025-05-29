<p>Leo didn't do all the job in his <a href="http://www.spoj.com/problems/DUKKAR2/">last problem</a>, somebody gave him the numbers in a convenient base. It was the bottleneck of the problem... Now your task is to do this job.
</p>

<h3>Input</h3>
<p>The first line of input contains three integers
 <strong><em>T</em></strong>, the number of test cases, 
 <strong><em>B1</em></strong>, the first base, 
 <strong><em>B2</em></strong>, the second base.<br> 
 
Follow 2¡Á<strong><em>T</em></strong> lines.<br>
For each test case, on the first line your are given one integer <strong><em>k</em></strong>.<br>
On the second line you are given <strong><em>k</em></strong> integers : the digits of <strong><em>N</em></strong> in base <strong><em>B1</em></strong>.<br>
<br>
<strong><em>N = a<sub>0</sub>¡ÁB1<sup>0</sup> + ... + a<sub>i</sub>¡ÁB1<sup>i</sup> + ... + a<sub>k-1</sub>¡ÁB1<sup>k-1</sup> </em></strong>
</p>

<h3>Output</h3>
<p>For each test case, you have to print the number <strong><em>N</em></strong> in base <strong><em>B2</em></strong>.
See sample for details.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
1 10 100
5
5 4 3 2 1
</pre>
<pre><strong>Output:</strong>
3
45 23 1
</pre>
<h3>Explanations</h3>
<p>For the lonely case, N = 5¡Á10<sup>0</sup> + 4¡Á10<sup>1</sup> + 3¡Á10<sup>2</sup> + 2¡Á10<sup>3</sup> + 1¡Á10<sup>4</sup> = 12345.<br>
We have: N = 45¡Á100<sup>0</sup> + 23¡Á100<sup>1</sup> + 1¡Á100<sup>2</sup>. You have to print 3, the number of digits,
 then the digits: 45, 23 and 1.<br>

</p><h3>Constraints</h3>
<pre>0 &lt; T &lt;= 50
1 &lt; B1,B2 &lt;= 10^9
1 &lt; k &lt;= 10000
0 &lt;= a<sub>i</sub> &lt; B1  , a<sub>k-1</sub>&gt;0
</pre>
<p>Time limit is sqrt(T_basic_pike_code * T_awaited_python_code) = sqrt(13.34*6.97), based on my Python3/Pike experiments.<br>
You may try before the <a href="http://www.spoj.com/problems/BASECVT/">tutorial edition</a>.<br>
<strong>Have fun ;-)</strong></p>
<p></p>
Edit(2017-02-11) : With compiler updates, a new time limit is set.<br>
Time limit is sqrt(T_basic_pike_code * T_awaited_python_code) = sqrt(3.93*1.57), based on my Python3/Pike experiments.<br>
Thanks @Blue_Mary for pointing this out.