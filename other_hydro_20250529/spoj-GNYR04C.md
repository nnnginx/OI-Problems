<p style="font-family: 'Times New Roman'; font-size: medium;">Lotto is a lottery, typically with an accumulating jackpot, in which participants play numbers of their choice in a random drawing. Lenny likes to play the lotto in Lincoln county Louisiana. In the game, he picks a list of&nbsp;<span><em>n</em></span>&nbsp;numbers in the range from 1 to&nbsp;<span><em>m</em></span>. If his list matches the drawn list, he wins the big prize, a lifetime supply of large lemons.</p>
<p style="font-family: 'Times New Roman'; font-size: medium;">Lenny has a scheme that he thinks is likely to be lucky. He likes to choose his list so that each number in it is at least twice as large as the one before it. So, for example, if&nbsp;<span><em>n</em>&nbsp;= 4</span>&nbsp;and&nbsp;<span><em>m</em>&nbsp;= 10</span>, then the possible lucky lists Lenny could pick are:</p>
<pre>    1 2 4 8
    1 2 4 9
    1 2 4 10
    1 2 5 10
</pre>
<p style="font-family: 'Times New Roman'; font-size: medium;">Thus Lenny has 4 lists to choose from.</p>
<p style="font-family: 'Times New Roman'; font-size: medium;">Your job, given&nbsp;<span><em>n</em></span>&nbsp;and&nbsp;<span><em>m</em></span>, is to count how many lucky lists Lenny has to his disposal.</p>
<p><br></p>

<h1><span style="color: #ff0000; font-size: medium;">Input</span></h1>
<p style="font-family: 'Times New Roman'; font-size: medium;">The first line of input is a single non-negative integer, which is the number of data sets to follow. All data sets should be handled identically. The next lines, one per data set, contain two integers,&nbsp;<span><em>n</em></span>and&nbsp;<span><em>m</em></span>. It is guaranteed that&nbsp;<span>1 &lt;= <em>n</em> &lt;= 10</span>&nbsp;and&nbsp;<span>1 &lt;= <em>m</em> &lt;= 2000</span>&nbsp;and <span><em>n</em> &lt;= <em>m</em></span>.</p>
<p><br></p>

<h1><span style="color: #ff0000; font-size: medium;">Output</span></h1>
<p style="font-family: 'Times New Roman'; font-size: medium;">For each data set, print a line like the following:</p>
<p style="font-family: 'Times New Roman'; font-size: medium;"><tt>Data set&nbsp;<span><em>i</em></span>:&nbsp;<span><em>n</em>&nbsp;<em>m</em>&nbsp;<em>number</em></span></tt></p>
<p style="font-family: 'Times New Roman'; font-size: medium;">where&nbsp;<span><em>i</em></span>&nbsp;is the data set number (beginning with 1), and&nbsp;<span><em>number</em></span>&nbsp;is the maximum number of lucky lists corresponding to the provided values of&nbsp;<span><em>n</em></span>&nbsp;and&nbsp;<span><em>m</em></span>.</p>
<p><br></p>

<h1><span style="color: #ff0000; font-size: medium;">Example</span></h1>
<p><span style="color: #ff0000; font-size: small;">Input</span></p>
<pre>1
4 10</pre>
<p><span style="color: #ff0000; font-size: small;">Output</span></p>
<pre>Data set 1: 4 10 4</pre>