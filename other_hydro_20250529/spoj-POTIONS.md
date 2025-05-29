<p style="font-family: Arial, sans-serif; font-size: 13px; line-height: 18px;">Its time for the Potions class. Harry absolutely HATES potions because he has to face mockery by the potions teacher Snape everytime he has a potions class. Snape never leaves any chance of insulting him in front of everyone.</p>
<p style="font-family: Arial, sans-serif; font-size: 13px; line-height: 18px;">Snape is not in a good mood today, which is not good for Harry. Snape challenges Harry to answer his question. If Harry fails to answer, he will have to spend the whole week in detention!.</p>
<p style="font-family: Arial, sans-serif; font-size: 13px; line-height: 18px;">He gives Harry n numbers ( a1, a2, a3,...., an ) and q queries. Each query will consist of four integers,<strong>w, x, y, z</strong>&nbsp;. The result of a query is given by the following equation:</p>
<p style="font-family: Arial, sans-serif; font-size: 13px; line-height: 18px;"><img title="Equation" src="../../../content/abhinav92003:equation_potions" alt="Equation" width="173" height="77"></p>
<p style="font-family: Arial, sans-serif; font-size: 13px; line-height: 18px;"><span style="font-family: Arial, sans-serif; font-size: 13px; line-height: 18px;">Help Harry or else he'll miss his Quidditch match against Slytherin because of his detention..!!</span></p>
<h3>Input</h3>
<p style="font-family: Arial, sans-serif; font-size: 13px; line-height: 18px;">The first line of the input contains&nbsp;<strong>T</strong>, the number of test cases.&nbsp;<strong>T</strong>&nbsp;test cases follow.</p>
<p style="font-family: Arial, sans-serif; font-size: 13px; line-height: 18px;">The first line of each test case contains&nbsp;<strong>n</strong>&nbsp;and&nbsp;<strong>q</strong>.</p>
<p style="font-family: Arial, sans-serif; font-size: 13px; line-height: 18px;">The second line of each test case contains&nbsp;<strong>n</strong>&nbsp;integers&nbsp;<strong>(a1, a2, a3,..,an)</strong></p>
<p style="font-family: Arial, sans-serif; font-size: 13px; line-height: 18px;">Each of the next&nbsp;<strong>q</strong>&nbsp;lines contain&nbsp;<strong>w, x, y, z</strong>.</p>
<h3>Output</h3>
<p style="font-family: Arial, sans-serif; font-size: 13px; line-height: 18px;">For each test case output the result as given by the equation.</p>
<p style="font-family: Arial, sans-serif; font-size: 13px; line-height: 18px;">The answer may be very large, so output it&nbsp;<strong>modulo 10^9+7</strong></p>
<p style="font-family: Arial, sans-serif; font-size: 13px; line-height: 18px;"><strong>Constraints:</strong></p>
<p style="font-family: Arial, sans-serif; font-size: 13px; line-height: 18px;">1&lt;=&nbsp;<strong>T</strong>&nbsp;&lt;=10</p>
<p style="font-family: Arial, sans-serif; font-size: 13px; line-height: 18px;">1&lt;=&nbsp;<strong>n, q</strong>&nbsp;&lt;=10^5</p>
<p style="font-family: Arial, sans-serif; font-size: 13px; line-height: 18px;">1&lt;=&nbsp;<strong>x+i</strong>&nbsp;&lt;=n ( for all y&lt;=i&lt;=z )</p>
<p style="font-family: Arial, sans-serif; font-size: 13px; line-height: 18px;">0&lt;=&nbsp;<strong>ai</strong>&nbsp;&lt;=10^9 ( for all 1&lt;=i&lt;=n)</p>
<p style="font-family: Arial, sans-serif; font-size: 13px; line-height: 18px;">1&lt;=&nbsp;<strong>w</strong>&nbsp;&lt;=10^6</p>
<p style="font-family: Arial, sans-serif; font-size: 13px; line-height: 18px;"><strong>0&lt;=y&lt;=z</strong></p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<span style="font-family: Arial, sans-serif; font-size: 13px; line-height: 18px;">1</span><br style="font-family: Arial, sans-serif; font-size: 13px; line-height: 18px;"><span style="font-family: Arial, sans-serif; font-size: 13px; line-height: 18px;">5 2</span><br style="font-family: Arial, sans-serif; font-size: 13px; line-height: 18px;"><span style="font-family: Arial, sans-serif; font-size: 13px; line-height: 18px;">2 1 4 7 2</span><br style="font-family: Arial, sans-serif; font-size: 13px; line-height: 18px;"><span style="font-family: Arial, sans-serif; font-size: 13px; line-height: 18px;">1 1 0 2</span><br style="font-family: Arial, sans-serif; font-size: 13px; line-height: 18px;"><span style="font-family: Arial, sans-serif; font-size: 13px; line-height: 18px;">1 5 0 0</span></pre>
<pre><strong>Output:</strong>
<span style="font-family: Arial, sans-serif; font-size: 13px; line-height: 18px;">16</span><br style="font-family: Arial, sans-serif; font-size: 13px; line-height: 18px;"><span style="font-family: Arial, sans-serif; font-size: 13px; line-height: 18px;">2</span></pre>