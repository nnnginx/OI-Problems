<p>A trick sometimes used by parents to teach their children the value of money is to give then a penny – just
a penny! – and the promise that for each day they don’t spend it, the parent will double it. All students of
computing know that long before a month has elapsed without spending a cent, the parents will not likely be
able to make good on their promise.

</p><p></p><p>
100-percent compound daily interest on an investment is, of course, unattainable in normal financial
dealings, but we are all continually reminded of the power of compound interest, even with the relatively
low interest rates available today.

</p><p></p><p>
But exactly how much money can be made with compound interest? Assume, for example, an initial
investment of $100.00 (US or Canadian ☺), an annual interest rate of 6.00 percent, and that interest is
compounded monthly. That is, the interest earned during the preceding month is added to the principal at
the end of the month. (For our purposes, we’ll assume a month is exactly 1/12th of a year.)

</p><p></p><p>
At the end of the first month, the money will have earned 0.5 percent interest (1/12th of 6.00 percent), or
$0.50. This is added to the $100.00 invested, so that during the next month, interest is paid on $100.50.
During the next month another 0.5 percent interest is earned, which is exactly $0.5025. We will assume
that the bank, being conservative, will not pay any interest less than $0.01, so our investment is credited
with an additional $0.50 at the end of the second month, for a whopping total of $101.00. Continuing in the
same manner, at the end of 12 months our investment will total $106.12, $0.12 more than simple 6.00
percent interest for a year with no compounding.

</p><p></p><p>
Given an amount P to be invested for a year with I percent interest, compounded C times during the year at
equal intervals, what is total return on the investment?

</p><h3>Input</h3>
<p>There will be multiple cases to consider. The input for each case is a single line containing the initial
investment amount, P, given in dollars and cents (but no fractional cents, and no larger than $100,000.00),
the annual interest rate (I) given as a real number with two fractional digits representing a percentage,
greater than zero but less than 100, and the number of compounding intervals per year (C), an integer
between 1 and 365. The last case will be followed by a line containing “0.00 0.00 0”.

</p><h3>Output</h3>
<p>For each input case, display the case number (1, 2, …), the initial investment (P), the annual interest rate
(I), the number of compounding intervals per year(C), and the value of the investment at the end of a year.
Your output should follow the format shown in the examples below.

</p><h3>Example</h3>

<pre><b>Input:</b>
100.00 6.00 1
100.00 6.00 12
1000.00 6.00 12
0.00 0.00 0

<b>Output:</b>
Case 1. $100.00 at 6.00% APR compounded 1 times yields $106.00
Case 2. $100.00 at 6.00% APR compounded 12 times yields $106.12
Case 3. $1000.00 at 6.00% APR compounded 12 times yields $1061.63
</pre>