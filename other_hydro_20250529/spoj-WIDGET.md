<p>The widget factory produces several different kinds of widgets. Each widget is carefully built by a skilled widgeteer. The time required to build a widget depends on its type: the simple widgets need only 3 days, but the most complex ones may need as many as 9 days. 
</p><p>The factory is currently in a state of complete chaos: recently, the factory has been bought by a new owner, and the new director has fired almost everyone. The new staff know almost nothing about building widgets, and it seems that no one remembers how many days are required to build each diofferent type of widget. This is very embarrassing when a client orders widgets and the factory cannot tell the client how many days are needed to produce the required goods. Fortunately, there are records that say for each widgeteer the date when he started working at the factory, the date when he was fired and what types of widgets he built. The problem is that the record does not say the exact date of starting and leaving the job, only the day of the week. Nevertheless, even this information might be helpful in certain cases: for example, if a widgeteer started working on a Tuesday, built a Type 41 widget, and was fired on a Friday,then we know that it takes 4 days to build a Type 41 widget. Your task is to figure out from these records (if possible) the number of days that are required to build the different types of widgets. </p>
<h3>Input</h3>
<p>The input contains several blocks of test cases. Each case begins with a line containing two integers: the number 1 &lt;= n &lt;= 300 of the different types, and the number 1 &lt;= m &lt;= 300 of the records. This line is followed by a description of the m records. Each record is described by two lines. The first line contains the total number 1 &lt;= k &lt;= 10000 of widgets built by this widgeteer, followed by the day of week when he/she started working and the day of the week he/she was fired. The days of the week are given bythe strings 'MON', 'TUE', 'WED', 'THU', 'FRI', 'SAT' and 'SUN'. The second line contains k integers separated by spaces. These numbers are between 1 and n , and they describe the diofferent types of widgets that the widgeteer built. For example, the following two lines mean that the widgeteer started working on a Wednesday, built a Type 13 widget, a Type 18 widget, a Type 1 widget, again a Type 13 widget,and was fired on a Sunday. </p>
<pre>4 WED SUN 
13 18 1 13 
</pre>
<p>Note that the widgeteers work 7 days a week, and they were working on every day between their first and last day at the factory (if you like weekends and holidays, then do not become a widgeteer!).
</p><p>The input is terminated by a test case with n = m = 0 . </p>
<h3>Output</h3>
<p>For each test case, you have to output a single line containing n integers separated by spaces: the number of days required to build the different types of widgets. There should be no space before the first number or after the last number, and there should be exactly one space between two numbers. If there is more than one possible solution for the problem, then write 'Multiple solutions.' (without the quotes). If you are sure that there is no solution consistent with the input, then write 'Inconsistent data.'(without the quotes).</p>
<h3>Example</h3>
<pre><b>Input:</b>
2 3
2 MON THU
1 2
3 MON FRI
1 1 2
3 MON SUN
1 2 2
10 2
1 MON TUE 
3
1 MON WED
3
0 0

<b>Output:</b>
8 3
Inconsistent data.
</pre>
<b>Warning: large input/output data, be careful with certain languages</b>