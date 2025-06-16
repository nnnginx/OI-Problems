<p><span style="font-weight: bold; font-family: verdana, geneva;">Charlie and the Chocolate Factory</span></p>
<p><span style="font-family: verdana, geneva;"> </span></p>
<p><span style="font-family: verdana, geneva;">Charlie Bucket is a loving and kind boy, who lives in poverty with his mother, father and four bedridden grandparents. Down the street, there is Willy Wonka¡¯s chocolate factory who is famous for both his chocolates and the factory. After long years of conducting business with chocolate, now Wonka finally decided to make an heir to the factory.</span></p>
<p><span style="font-family: verdana, geneva;"> </span></p>
<p><span style="font-family: verdana, geneva;">So, instead of putting golden tickets in ordinary Wonka bars (which is old fashioned¡­.:P) he decided to take a programming contest to choose 5 candidates for the heir. And, then he will give a tough problem to them (among these five) and the first to answer will be the winner.</span></p>
<p><span style="font-family: verdana, geneva;"> </span></p>
<p><span style="font-family: verdana, geneva;">After taking the contest Wonka eventually gets his five candidates and Charlie is one of them.Now, before throwing the heir deciding problem towards them he decided to give them 2 hints.</span></p>
<p><span style="font-family: verdana, geneva;"> </span></p>
<p><span style="font-family: verdana, geneva;">1st hint is an algorithm whose pseudo code is given below</span></p>
<p><span style="font-family: verdana, geneva;"> </span></p>
<p><span style="font-family: verdana, geneva;"> <img src="file://MsUUg37I.png" alt="Pseudo Code">&nbsp;</span></p>
<pre># `array` is 1-indexed
def MakeNewArray(array, d):
  if d == 1:
    return array
  else:
    array = MakeNewArray(array, d-1)
    new_array = [array[array[i]] for i in 1..inf]
    return new_array
</pre>
<p>For example, if <tt>array = [2, 3, 5, 7, 11, ...]</tt>, then <tt>MakeNewArray(array, 2) = [3, 5, 11, ...]</tt>.
</p><p><span style="font-family: verdana, geneva;"> </span></p>
<p><span style="font-family: verdana, geneva;">2nd hint is <strong>Kuddus</strong> array. A <strong>Kuddus</strong> array is a sorted array of <strong>Kuddus</strong> numbers. <strong>Kuddus</strong> numbers are such <strong>prime</strong> numbers which can be expressed as the summation of squares of two distinct positive integers.For, example 5 can be expressed as 1<sup>2</sup>+2<sup>2</sup>. So it is a <strong>Kuddus</strong> number. Also 13(3<sup>2</sup>+2<sup>2</sup>) and 17(4<sup>2</sup>+1<sup>2</sup>) are <strong>Kuddus</strong> number. So, first few numbers of <strong>Kuddus</strong> array are 5,13,17¡­. etc.</span></p>
<p><span style="font-family: verdana, geneva;"> </span></p>
<p><span style="font-family: verdana, geneva;">Now, it¡¯s time for the heir deciding problem. The problem is as follows. There are <strong>n</strong> boxes and all of them are initially empty(no chocolate). Now in every step (starts from 1st step to the last) Wonka will do some sets of operation. The operation are of four kinds. The operation is indicated by an integer<strong> op</strong>.</span></p>
<p><span style="font-family: verdana, geneva;"> </span></p>
<p><span style="font-family: verdana, geneva;">i)&nbsp; If <strong>op=1</strong>. Then it is an add operation and it is followed by two integers <strong>a,b</strong>. It means Wonka will&nbsp;&nbsp;&nbsp; add <strong>b</strong> chocolates in box number <strong>a</strong>.</span></p>
<p><span style="font-family: verdana, geneva;"> </span></p>
<p><span style="font-family: verdana, geneva;">ii) If <strong>op=2</strong>. Then it is a multiplication operation which is also followed by two integers <strong>a,b</strong>. It means Wonka will multiply the number of chocolates in box number <strong>a</strong> by <strong>b</strong>.</span></p>
<p><span style="font-family: verdana, geneva;"> </span></p>
<p><span style="font-family: verdana, geneva;">iii) If <strong>op=3</strong>. Then it is a swap operation which is also followed by <strong>a,b</strong>. It means the boxes <strong>a </strong>and <strong>b</strong> will exchange their chocolates.</span></p>
<p><span style="font-family: verdana, geneva;"> </span></p>
<p><span style="font-family: verdana, geneva;">iv) If <strong>op=4</strong>. Then it is a clear operation which is followed by only a single integer <strong>a</strong>. This means Wonka will remove all chocolates from box <strong>a</strong>.</span></p>
<p><span style="font-family: verdana, geneva;"> </span></p>
<p><span style="font-family: verdana, geneva;"> </span></p>
<p><span style="font-family: verdana, geneva;">There are<strong> 2</strong> sets of operation. One is an <strong>ordinary</strong> set and another is <strong>special</strong> set. In normal steps he will perform the <strong>ordinary</strong> set of operation serially (as it appears in the input). And in the special steps he will perform the <strong>special</strong> set of operation serially. Special step number is stored in an array called <strong>Special </strong>array.</span></p>
<p><span style="font-family: verdana, geneva;"> </span></p>
<p><span style="font-family: verdana, geneva;">More precisely, he has an array named <strong>Special</strong> of infinite numbers. It is a sorted array. The elements of the array are denoted by <strong>Special[1],Special[2],Special[3]</strong>....etc [normal array system].So he will perform the special operation only at <strong>Special[1]th,Special[2]th, Special[3]th</strong>¡­... etc steps.</span></p>
<p><span style="font-family: verdana, geneva;"> </span></p>
<p><span style="font-family: verdana, geneva;">Now,</span></p>
<p><span style="font-family: verdana, geneva;"> </span></p>
<p><strong><span style="font-family: verdana, geneva;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Special:=MakeNewArray(Kuddus,d).</span></strong></p>
<p><span style="font-family: verdana, geneva;">Here <strong>MakeNewArray</strong> and <strong>Kuddus</strong> are described previously. <strong>d</strong> is an integer which will be given in the input. At last Wonka will tell the number of steps <strong>s</strong>.</span></p>
<p><span style="font-family: verdana, geneva;">Now, Charlie is busy in some other works. So, he needs your help. You will have to answer after <strong>s </strong>steps what is the total number of chocolates in all the boxes (summation of all the chocolates in every box).</span></p>
<p><strong><span style="font-family: verdana, geneva;">Input:</span></strong></p>
<p><span style="font-family: verdana, geneva;"> </span></p>
<p><span style="font-family: verdana, geneva;">Input consists of some test cases (not more than <strong>15</strong>).</span></p>
<p><span style="font-family: verdana, geneva;">Every case begins with two integer<strong> n (&gt;=2) </strong>and <strong>d (1&lt;=d&lt;=5)</strong>. Then there is an integer <strong>op1</strong> which denotes the number of operation for ordinary steps. The next <strong>op1</strong> lines each contain a number <strong>op</strong> <strong>(1&lt;=op&lt;=4)</strong> and if<strong> op&lt;=3</strong> then it is followed by two integers <strong>a</strong> and <strong>b</strong>, otherwise<strong> (op=4)</strong> it is followed by<strong> a</strong>. The meaning of them is described above. Then there is another integer <strong>op2</strong> which denotes the number of operations for special steps and the next <strong>op2</strong> steps is also followed by same format of input as <strong>op1</strong> is followed.Finally comes the number of steps <strong>s (1&lt;=s&lt;=10<sup>8</sup>)</strong>.</span></p>
<p><span style="font-family: verdana, geneva;"> </span></p>
<p><span style="font-family: verdana, geneva;">The meaning of every symbol is described above. Every input is a non-negative integer and not more than <strong>1000</strong> unless stated otherwise. There are no illegal input (i.e. there is no illegal box where operation will be performed). It is also guaranteed that there are equal number of cases for each possible values of <strong>d </strong>and <strong>n&lt;=2*d<sup>2</sup></strong>.</span></p>
<p><span style="font-family: verdana, geneva;"> </span></p>
<p><strong><span style="font-family: verdana, geneva;">Output:</span></strong></p>
<p><span style="font-family: verdana, geneva;"> </span></p>
<p><span style="font-family: verdana, geneva;">For each testcase the answer will be just a single line denoting the total number of chocolates in the boxes after <strong>s</strong> steps. You should return the <strong>answer%2<sup>64</sup></strong>.</span></p>
<p><span style="font-family: verdana, geneva;"><br></span></p>
<p><span style="font-family: verdana, geneva;"> </span></p>
<table style="width: 624px;" border="1" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td width="305" valign="top">
<p><strong><span style="font-family: verdana, geneva;">Sample Input</span></strong></p>
</td>
<td width="319" valign="top">
<p><strong><span style="font-family: verdana, geneva;">Sample Output</span></strong></p>
</td>
</tr>
<tr>
<td width="305" valign="top">
<pre>2 1
5
1 1 1
1 2 1
2 1 2
2 2 3
3 1 2
3
1 1 1
1 2 1
3 1 2
4

2 1
5
1 1 1
1 2 1
2 1 2
2 2 3
3 1 2
3
1 1 1
1 2 1
3 1 2
5</pre>
</td>
<td width="319" valign="top">
<pre>119
121</pre>
</td>
</tr>
</tbody>
</table>
<p><span style="font-family: verdana, geneva;"> </span></p>
<p>&nbsp;</p>
<p>Problem Setter: Syed Shahriar Manjur</p>
<p>Special Thanks: Nafis Ahmed</p>