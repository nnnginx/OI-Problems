<pre></pre>
<p>   </p>
<table style="width: 100%; background-color: #44c23c;" border="0">
<tbody>
<tr>
<td style="text-align: center;" width="50%"><a href="/problems/ANARC07G/en/">English</a></td>
<td style="text-align: center;" width="50%"><a href="/problems/ANARC07G/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p></p>
<p>A favorite pastime for big families in Acmestan is going to the movies. It is quite common to see a number of these multi-generation families going together to watch a movie. Movie theaters in Acmestan have two types of tickets: A single ticket is for exactly one person while a family ticket allows a parent and their children to enter the theater.&nbsp; Needless to say, a family ticket is always priced higher than a single ticket, sometimes as high as ﬁve times the price of a single ticket.</p>
<p>&nbsp;</p>
<p style="text-align: center;"><img src="../../../../../../content/simes:ANARC07G.png" alt=""></p>
<p style="text-align: justify;">&nbsp;</p>
<p style="text-align: justify;">It is quite challenging for families to decide which ticket arrangement is most economical to buy. For example, the family depicted in the ﬁgure on the right has four ticket arrangements to choose from: Seven single tickets; Two family tickets; One family ticket (for adam, bob, cindy)plus four single tickets for the rest; Or, one family ticket (for bob and his four children) plus single tickets for the remaining two.</p>
<p style="text-align: justify;"><br>Write a program to determine which ticket arrangement has the least price. If there are more than one such arrangement, print the arrangement that has the least number of tickets.</p>
<h1 style="text-align: center;">Input</h1>
<p>Your program will be tested on one or more test cases. The ﬁrst line of each test case includes two positive integers (S and F)where S is the price of a single ticket and F is the price of a family ticket. The remaining lines of the test case are either the name of a person going by him/herself, or of the form:</p>
<pre>N1 N2 N3 ... Nk<br></pre>
<p>where N1 is the name of a parent, with N2 ... Nk being his/her children. Names are all lower-case letters, and no longer than 1000 characters. No parent will be taking more than 1000 of their children to the movies :-). Names are unique, the name of a particular person will appear at most twice: Once as a parent, and once as a child. There will be at least one person and at most 100,000 people in any test case.</p>
<p>The end of a test case is identiﬁed by the beginning of the following test case (a line made of twointegers.) The end of the last test case is identiﬁed by two zeros.</p>
<h1 style="text-align: center;">Output</h1>
<p>For each test case, write the result using the following format:</p>
<pre>k. NS NF T</pre>
<p>Where k is the test case number (starting at 1,) NS is the number of single tickets, NF is the number of family tickets, and T is the total cost of tickets.</p>
<h1 style="text-align: center;">Sample</h1>
<pre style="text-align: justify;">input<br>1 3<br>adam bob cindy<br>bob dima edie fairuz gary<br>1 2<br>john<br>paul<br>george<br>ringo<br>1 3<br>a b c<br>0 0<br><br>output<br>1. 2 1 5<br>2. 4 0 4<br>3. 0 1 3</pre>
<p> </p>