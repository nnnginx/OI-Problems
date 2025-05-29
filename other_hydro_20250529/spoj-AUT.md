<p style="color: #444444; font-family: Tahoma, Arial; font-size: 12.800000190734863px; line-height: 17.600000381469727px;">Byteasar studies computer science at the University of Bytetown. There is a snack vending machine at his faculty that sells&nbsp;<b>n</b>&nbsp;types of snacks, numbered&nbsp;<b>1</b>&nbsp;through&nbsp;<b>n</b> Snacks of different types may have different price, since they differ in size and flavor.</p>
<p style="color: #444444; font-family: Tahoma, Arial; font-size: 12.800000190734863px; line-height: 17.600000381469727px;">Recently Byteasar discovered that the vending machine is broken. If one buys a snack of type&nbsp;<b>i</b>, the vending machine additionally dispenses one snack of each of the types&nbsp;<b>1</b>, <b>2</b>, <b>...</b>, <b>i-1</b>, provided that snacks of these types are available (if there are no snacks of some of the types&nbsp;<b>1</b>, <b>2</b>, <b>...</b>, <b>i-1</b>, simply no snack of this type is dispensed). Buying snack of type&nbsp;<b>i</b>&nbsp;is possible only if at least one snack of this type is available.</p>
<p style="color: #444444; font-family: Tahoma, Arial; font-size: 12.800000190734863px; line-height: 17.600000381469727px;">Byteasar decided to take advantage of the fault he discovered. He would like to find out what is the maximum total value (that is, the sum of prices) of snacks that he can obtain in the vending machine using a given amount of money. He does not have to use all the money.</p>
<h3>Input</h3>
<p>First line contains a single integer t representing the number of test cases to be solved. The description of t test cases follows.</p>

<p>The first line of each test case contains two integers <b>n</b> and <b>k</b> (1 &lt;= <b>n</b> &lt;= 40, 1 &lt;= <b>k</b> &lt;= 64000): the number of types of snacks and the amount of money that Byteasar has at his disposal. The second line holds <b>n</b> integers <b>c<sub>1<sub></sub></sub></b>, <b>...</b>, <b>c<sub>n<sub></sub></sub></b> (1 &lt;= <b>c<sub>i<sub></sub></sub></b> &lt;= 40), the prices of snacks of respective types. The third line holds <b>n</b> integers <b>l<sub>1<sub></sub></sub></b>, <b>...</b>, <b>l<sub>n<sub></sub></sub></b> (1 &lt;= <b>l<sub>i<sub></sub></sub></b> &lt;= 40), the quantities of snacks of respective types that are available in the vending machine.</p>
<h3>Output</h3>
<p><span style="color: #444444; font-family: Tahoma, Arial; font-size: 12.800000190734863px; line-height: 17.600000381469727px;">The output should contain one integer per test case: the total price of snacks that Byteasar can obtain in the vending machine using at most <b>k</b>&nbsp;units of money.</span></p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<pre style="color: #444444; font-size: 12.800000190734863px; line-height: 17.600000381469727px;">1</pre>
<pre style="color: #444444; font-size: 12.800000190734863px; line-height: 17.600000381469727px;">6 8
7 2 3 5 7 2
1 3 0 3 2 1</pre>
<strong>Output:</strong>&nbsp;</pre>
<pre>30</pre>
<pre style="text-align: center;"><em>Task author: Jakub Pachocki</em></pre>