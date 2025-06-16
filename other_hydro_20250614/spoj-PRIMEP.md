<p style="box-sizing: border-box; margin: 0px 0px 10px; color: #555555; font-family: &quot;Open Sans&quot;, &quot;Helvetica Neue&quot;, Helvetica, Arial, sans-serif; font-size: 14px;"><span style="box-sizing: border-box; font-weight: 700;">N</span>&nbsp;Slovakistan farmers own neighbouring fields alongside a river, forming a straight line. Each field is infested with (possibly zero) pests.</p>
<p style="box-sizing: border-box; margin: 0px 0px 10px; color: #555555; font-family: &quot;Open Sans&quot;, &quot;Helvetica Neue&quot;, Helvetica, Arial, sans-serif; font-size: 14px;">Thanks to ingenious Slovakistan science, each species of pest can be assigned a prime number. Each field can then be assigned a positive number, representative of the pests that are infesting it - the prime factorization of this number indicates which pests are present, with the powers of each prime number representing how strongly the field is infested with that pest. The resulting number indicates how much damage is done to the crops on that field.</p>
<p style="box-sizing: border-box; margin: 0px 0px 10px; color: #555555; font-family: &quot;Open Sans&quot;, &quot;Helvetica Neue&quot;, Helvetica, Arial, sans-serif; font-size: 14px;">To help the farmers, the government is planning to spray pesticide on some contiguous segment of fields. Due to environmental concerns, the pesticide can only be effective against a single species of pest. However, what segment of fields to spray and with what pesticide has given rise to a huge debate in the parliament - there simply isn't enough data to decide. Given <strong>Q </strong>proposals <strong>L R p</strong>, meaning that pesticide against the pest assigned prime number <strong>p </strong>could be sprayed on fields <strong>L </strong>through <strong>R</strong>, find out how much damage to crops it would prevent.</p>
<h3>Input</h3>
<p>The first line of input contains two integers <strong>N</strong>&nbsp;and <strong>Q </strong>(<strong>1 ¡Ü N,Q ¡Ü 500,000</strong>): the number of fields and the number of proposals.</p>
<p>The second line contains <strong>N </strong>numbers <strong>f</strong><sub><strong>1</strong></sub><strong>, ... , f</strong><sub><strong>N </strong></sub><strong>- </strong>the numbers assigned to the fields. They will be positive and not greater than <strong>10</strong><sup><strong>6</strong></sup>.</p>
<p><strong>Q </strong>lines follow, each containing three numbers <strong>L R p&nbsp;</strong>(<strong>1 &nbsp;¡Ü L ¡Ü R ¡Ü N, 1&nbsp;¡Ü p</strong><strong>&nbsp;¡Ü 10<sup>6</sup>,</strong>&nbsp;<strong>p</strong><strong>&nbsp;</strong>is a prime number), meaning that the government proposes to spray pesticide against pest <strong>p </strong>on fields [<strong>L,R</strong>]</p>
<h3>Output</h3>
<p>For each proposal <strong>L R p</strong>, output how much crop damage is mitigated; that is, output&nbsp; (<strong>f</strong><strong><sub>L</sub>&nbsp;+ ... + f<sub>R</sub></strong>&nbsp;- <strong>f</strong><strong>'</strong><sub><strong>L</strong></sub><strong>&nbsp;- ... - f'</strong><sub><strong>R</strong>&nbsp;</sub>), where <strong>f</strong><strong>'</strong><sub><strong>i</strong> </sub>is <strong>f<sub>i</sub>&nbsp;</strong>after all factors of <strong>p&nbsp;</strong>have been removed from it.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5 5
10 20 30 40 50
1 1 2
1 5 5
1 5 47
2 4 3
2 4 2
<strong>Output:</strong>
5
128
0
20
65
</pre>
<p>In the fourth proposal, the result is (20 + 30 + 40 - 20 - 10 - 40) = 20.</p>