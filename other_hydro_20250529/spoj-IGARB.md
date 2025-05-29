<p> Fred works as an IT consultant in an insurance company. As they always had a large amount of customers waiting and arguing at the front desk, management decided to deploy a ticket machine. Each customer would get a ticket with a number and there will be fancy LCD display over each desk showing the number of the next person. Fred was appointed to get this new enhancement working. <br><br>

Because Fred is lazy when it comes to manual labor and as an IT consultant he wouldn't lower himself to the level of some hardware technician (except when upgrading his own computer), he asked few technicians to install the displays and prepared himself just to plug in the ticket machine and try it out. Unfortunately (for Fred) the technicians, either inspired by Mr.Bean or because of their carelessness, installed the display upside-down. <br><br>

Being a software guy, Fred decided that the hardware should not be tampered with after it is installed (except for the case if he would be able to get back the technicians to repair it, but they were already angry at him for his nagging). Then he noted that from time to time the display shows a correct number even when it is upside-down. And hey, the ticket machine is an embedded device and contains a small processor! It would be just a sin for an IT guy not to try to meddle with it and try running an own version of Linux. Now we just need to figure out which readable numbers will the display show.</p>

<h3>Task specification</h3>
<p>
In the beginning the display shows the number 1 on its display. Each second the number shown is increased by 1. We see the display upside-down and thus not everything we see will make sense. Your task is to compute the K-th valid number we will see on the display. The digits the display uses are shown on the images below. An upside-down 1 still count as 1. The number we see may have leading zeroes ¨C e.g. turning the number 600 upside down leads to a valid number.<br><br>

<img src="/content/turbo:i0.gif">&nbsp; 
<img src="/content/turbo:i1.gif">&nbsp; 
<img src="/content/turbo:i2.gif"> &nbsp;
<img src="/content/turbo:i3.gif"> &nbsp;
<img src="/content/turbo:i4.gif"> &nbsp;
<img src="/content/turbo:i5.gif"> &nbsp;
<img src="/content/turbo:i6.gif"> &nbsp;
<img src="/content/turbo:i7.gif"> &nbsp;
<img src="/content/turbo:i8.gif"> &nbsp;
<img src="/content/turbo:i9.gif">&nbsp;
</p>

<h3>Input</h3>
<p>
t - the number of test cases [t &lt;= 2200], than t test cses follows. Each test case consist of one integer Ki [0 &lt; Ki &lt;= 10^200].
</p>

<h3>Output</h3>
<p>For each Ki from the input file, output the Ki-th number shown on the display (including the leading zeroes, if there are some).
<br>  
</p>

<h3>Example</h3>
<pre><b>Input:</b>
8
1
2
3
4
5
6
8
98
</pre>
<pre><b>Output:</b>
1
2
5
9
8
6
11
002
</pre>