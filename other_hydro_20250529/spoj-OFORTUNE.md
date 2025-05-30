<p>
The Ohgas are a prestigious family based on Hachioji. The head of the family, Mr. Nemochi Ohga, a famous wealthy man, wishes to increase his fortune by depositing his money to an operation company. You are asked to help Mr. Ohga maximize his profit by operating the given money during a specified period. 
<br>
<br>From a given list of possible operations, you choose an operation to deposit the given fund to. You commit on the single operation throughout the period and deposit all the fund to it. Each operation specifies an annual interest rate, whether the interest is simple or compound, and an annual operation charge. An annual operation charge is a constant not depending on the balance of the fund. The amount of interest is calculated at the end of every year, by multiplying the balance of the fund under operation by the annual interest rate, and then rounding off its fractional part. For compound interest, it is added to the balance of the fund under operation, and thus becomes a subject of interest for the following years. For simple interest, on the other hand, it is saved somewhere else and does not enter the balance of the fund under operation (i.e. it is not a subject of interest in the following years). An operation charge is then subtracted from the balance of the fund under operation. You may assume here that you can always pay the operation charge (i.e. the balance of the fund under operation is never less than the operation charge). The amount of money you obtain after the specified years of operation is called ``the final amount of fund.'' For simple interest, it is the sum of the balance of the fund under operation at the end of the final year, plus the amount of interest accumulated throughout the period. For compound interest, it is simply the balance of the fund under operation at the end of the final year. 
<br>
<br>Operation companies use C, C++, Java, etc., to perform their calculations, so they pay a special attention to their interest rates. That is, in these companies, an interest rate is always an integral multiple of 0.0001220703125 and between 0.0001220703125 and 0.125 (inclusive). 0.0001220703125 is a decimal representation of 1/8192. Thus, interest rates' being its multiples means that they can be represented with no errors under the double-precision binary representation of floating-point numbers. 
<br>
<br>For example, if you operate 1000000 JPY for five years with an annual, compound interest rate of 0.03125 (3.125 %) and an annual operation charge of 3000 JPY, the balance changes as follows.

<br></p><table border=""><tbody><tr align="right" rowspan="2"><td>The balance of the fund under operation(at the beginning of year)</td><td>Interest</td><td>The balance of the fund under operation (at the end of year)</td></tr><tr align="right"><td>A</td><td>B = A �� 0.03125 (and rounding off fractions)</td><td>A + B - 3000</td></tr><tr align="right"><td>1000000</td><td>31250</td><td>1028250</td></tr><tr align="right"><td>1028250</td><td>32132</td><td>1057382</td></tr><tr align="right"><td>1057382</td><td>33043</td><td>1087425</td></tr><tr align="right"><td>1087425</td><td>33982</td><td>1118407</td></tr><tr align="right"><td>1118407</td><td>34950</td><td>1150357</td></tr></tbody></table>

<br>After the five years of operation, the final amount of fund is 1150357 JPY. 
<br>
<br>If the interest is simple with all other parameters being equal, it looks like: 
<br><table border=""><tbody><tr align="right" rowspan="2"><td>The balance of the fund under operation (at the beginning of year)</td><td>Interest</td><td>The balance of the fund under operation (at the end of year)</td><td>Cumulative interest </td></tr><tr align="right"><td>A</td><td>B = A �� 0.03125 (and rounding off fractions)</td><td>A - 3000</td><td></td></tr><tr align="right"><td>1000000</td><td>31250</td><td>997000</td><td>31250</td></tr><tr align="right"><td>997000</td><td>31156</td><td>994000</td><td>62406</td></tr><tr align="right"><td>994000</td><td>31062</td><td>991000</td><td>93468</td></tr><tr align="right"><td>991000</td><td>30968</td><td>988000</td><td>124436</td></tr><tr align="right"><td>988000</td><td>30875</td><td>985000</td><td>155311</td></tr></tbody></table>

<br>In this case the final amount of fund is the total of the fund under operation, 985000 JPY, and the cumulative interests, 155311 JPY, which is 1140311 JPY. <p></p>

<h3>Input</h3>
<p>
The input consists of datasets. The entire input looks like: 
<br></p><ul>the number of datasets (=m) 
<br>1st dataset 
<br>2nd dataset 
<br>... 
<br>m-th dataset </ul>
<br>The number of datasets, m, is no more than 100. Each dataset is formatted as follows. 
<br><ul>the initial amount of the fund for operation 
<br>the number of years of operation 
<br>the number of available operations (=n) 
<br>operation 1 
<br>operation 2 
<br>... 

<br>operation n </ul>
<p><br>The initial amount of the fund for operation, the number of years of operation, and the number of available operations are all positive integers. The first is no more than 100000000, the second no more than 10, and the third no more than 100. 
<br></p><ul>Each ``operation'' is formatted as follows. </ul>
<br><p>simple-or-compound annual-interest-rate annual-operation-charge 
<br>where simple-or-compound is a single character of either '0' or '1', with '0' indicating simple interest and '1' compound. annual-interest-rate is represented by a decimal fraction and is an integral multiple of 1/8192. annual-operation-charge is an integer not exceeding 100000. </p>
<br>

<h3>Output</h3>
<p>
For each dataset, print a line having a decimal integer indicating the final amount of fund for the best operation. The best operation is the one that yields the maximum final amount among the available operations. Each line should not have any character other than this number.

</p><p></p><p>
You may assume the final balance never exceeds 1000000000. You may also assume that at least one operation has the final amount of the fund no less than the initial amount of the fund. 

</p><h3>Example</h3>

<pre><b>Input:</b>
4
1000000
5
2
0 0.03125 3000
1 0.03125 3000
6620000
7
2
0 0.0732421875 42307
1 0.0740966796875 40942
39677000
4
4
0 0.0709228515625 30754
1 0.00634765625 26165
0 0.03662109375 79468
0 0.0679931640625 10932
10585000
6
4
1 0.0054931640625 59759
1 0.12353515625 56464
0 0.0496826171875 98193
0 0.0887451171875 78966

<b>Output:</b>
1150357
10559683
50796918
20829397
</pre>