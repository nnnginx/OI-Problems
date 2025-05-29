<p>Rabbits  are  incredible  animals.  One  of  their  more   interesting characteristics  is  related with  their  reproduction. If  we  keep a couple  of  adult  rabbits  in  optimal  conditions  of  life,  it  is scientifically  proved that,  each month,  that couple  is capable  of procreating a new couple of  young rabbits. You should know  that only the adult couples  may procreate and  that the time  taken by a  young couple of rabbits to  grow (that is, to  become adult) is of  1 month. For the  convenience of  this task,  we will  be dealing with immortal rabbits.</p>

<p>Farmer Luis  (FL) is  a great  admirer of  rabbits. FL  bought in  the market 1 couple of adult rabbits (alive, of course) and know wants  to raise as  many rabbits  as he  can. Unfortunately,  there is  a little problem, FL has boxes where he can only put exactly 2^M (1 &lt;= M &lt;= 20) couples of rabbits (neither more nor  less). FL can use as many  boxes as he wishes as long as he fulfils the condition above. FL would  like to know how many couples of rabbits he will not be able to put  inside boxes if he  raises rabbits for  N (1 &lt;=  N &lt;= 2147483647)  months and then tries to ¡®box¡¯ them (put  them inside boxes). You should help  FL with these calculations. You must consider that FL starts with 1 adult couple of rabbits the 1st month, and that couples of rabbits reproduce and grow as stated in the 1st paragraph.</p>

<h3>Input</h3>
<p>Line 1: C  (1 &lt;= C &lt;= 100), the number of calculations your program will be requested to do</p>
<p>Lines 2-C+1: two integers N and M (in that order)</p>

<h3>Output</h3>
<p>Lines 1-C: on each lines print S, which is the number of un-'boxed' couples of rabbits.</p>

<h3>Example</h3>
<pre><b>Input:</b>
1
5 2

<b>Output:</b>
0</pre>

<h3>Output explanation</h3>

<p>After  growing couples  of rabbits  during 5  months, FL  has 5  adult couples and 3 young couples (8  couples in total). FL has boxes where can put 2^2 = 4 couples of rabbits, so he can use 2 boxes to ¡®box¡¯ all the 8 couples.  If FL had instead grown couples of rabbits  for 4 months, he would  have 5 couples in total; thus 1 couple would have remained un-¡®boxed¡¯ (the answer would have been 1). </p>