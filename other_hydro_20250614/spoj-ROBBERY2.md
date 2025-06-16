<p><b>k</b> bandits robbed a bank. They took away <b>n</b> gold coins. Being a progressive group of robbers they decided to use the following procedure to divide the coins. First the most respected bandit takes <b>1</b> coin, then the second respected takes <b>2</b> coins, ..., the least respected takes <b>k</b> coins, then again the most respected takes <b>k+1</b> coins, ans so on, until one of the bandits takes the remaining coins. Calculate how much gold each of the bandits gets.

</p><h3>Input</h3>
<p>The first line of the input contains number <b>t</b> ¨C the amount of tests. Then <b>t</b> test descriptions follow. Each test consists of two integers <b>n</b> and <b>k</b> - the amount of coins and bandits respectively.

</p><h3>Constraints</h3>
<p>
1 &lt;= <b>t</b> &lt;= 500<br>
10<sup>6</sup> &lt;= <b>n</b> &lt;= 10<sup>15</sup><br>
2 &lt;= <b>k</b> &lt;= 100
</p>

<h3>Output</h3>
<p>For each test print the amounts of coins each bandit gets separated by spaces.

</p><h3>Example</h3>

<pre><b>Input:</b>
3
1000000 2
1234567 3
123456789 4

<b>Output:</b>
499849 500151
411602 411887 411078
30869901 30858368 30862296 30866224

</pre>