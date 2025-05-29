<p>A company uses temporary employees (¡°temps¡±) to handle its varying workloads. By doing so, it avoids having
to pay for benefits normally provided to its permanent employees. However, the company must pay an
employment agency a fixed fee for each temp they hire, as well as paying the temp a fixed amount of
severance pay when they are terminated ¨C in addition, of course, to the monthly salary each temp receives.
The company has a good understanding of when it needs temporary workers, and how many such workers it
will require each month. Depending on the fee paid to the employment agency, the temporary worker¡¯s
salary, and the severance pay, it may make sense to retain an unneeded worker for one or more months if
it¡¯s known that they will be needed again in the future.

</p><p></p><p>
Let¡¯s consider an example. Suppose we know that in March the company will need 10 temps, in April they¡¯ll
need 9, and in May they¡¯ll need 11. Suppose a temp earns $500 per month, that the employment agency
receives $400 for each temp hired, and $600 is paid as severance to each temp that is terminated. If the
company employs just the minimum number of temps required, then their payments will be as follows (we
ignore the cost of terminating all employees at the end of the last month):

</p><p></p><p>
</p><center><img src="/content/steinersp:budget.jpg" alt="Illustration" border="0" width="100%"></center>
<p></p><p>

The total cost to the company is $20,400. But suppose they did not terminate the unneeded temp at the
end of March, but just let that person remain employed. They would then save $400 in employment agency
fees (since they¡¯d need to hire just one additional temp for May), $600 in severance pay, and only have to
pay the temp worker $500, for an overall savings of $500.

</p><p></p><p>
In this problem you are given, as input, the number of months for which the company is to plan its temp
worker budget, the cost of hiring and firing a temp worker, the temp worker¡¯s monthly salary, and the
required minimum number of workers needed each month. You are to determine the minimum cost to the
company to have at least the required minimum number of workers on hand each month. Assume there are
no temporary workers on hand before the first month, and that the cost of terminating the workers at the
end of the last month is not to be included in the cost. You may assume that the planning interval will be no
longer than 24 months, and the hiring cost, severance pay, and monthly salary for each temp worker is
greater than zero.

</p><h3>Input</h3>
<p>There will be multiple cases to consider. The input for each case begins with an integer N, the number of
months for which planning is required (never larger than 24). This is followed by three integers giving the
cost of hiring a worker, the worker¡¯s monthly salary, and the severance pay for a terminated worker. Finally
there will appear N integers giving the required minimum number of workers needed in each month. The last
case will be followed by a zero.

</p><h3>Output</h3>
<p>For each input case, display the case number (1, 2, ¡­) and the minimum cost to the company. Use the format
shown in the examples below.

</p><h3>Example</h3>

<pre><b>Input:</b>
3 400 500 600 10 9 11
8 400 600 600 11 9 10 14 9 9 13 15
0

<b>Output:</b>
Case 1, cost = $19900
Case 2, cost = $66600
</pre>