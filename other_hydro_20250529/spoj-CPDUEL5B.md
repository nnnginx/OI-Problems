<p style="font-family: 'Ubuntu', sans-serif; font-size: 14px;">Watame needs to consume asacoco. However, consuming too much asacoco can be dangerous, so she consults with a doctor.</p>
<p style="font-family: 'Ubuntu', sans-serif; font-size: 14px;">The doctor recommends her a limit for every day. Let <strong>A<sub>i&nbsp;</sub></strong>be <strong>a real number</strong> denoting the limit of asacoco allowed to be consumed in the <strong>i</strong>-th day.</p>
<p style="font-family: 'Ubuntu', sans-serif; font-size: 14px;">Uniquely, the array <strong>A</strong><sub>i</sub><sub>&nbsp;</sub>is a non-decreasing arithmetic sequence.</p>
<p style="font-family: 'Ubuntu', sans-serif; font-size: 14px;">An element&nbsp;<strong><strong>A</strong><sub><sub>i</sub> </sub></strong><span style="font-family: Ubuntu, sans-serif; font-weight: bold;">c</span><span style="font-family: Ubuntu, sans-serif; font-weight: bold;">an be represented as</span><span style="font-family: Ubuntu, sans-serif; font-weight: bold;"> <strong>A<sub>0</sub><sub>&nbsp;</sub>+ i * d</strong>&nbsp;</span><span style="font-family: Ubuntu, sans-serif; font-weight: bold;">where</span><span style="font-family: Ubuntu, sans-serif; font-weight: bold;"> <strong>d</strong>&nbsp;</span><span style="font-family: Ubuntu, sans-serif; font-weight: bold;">is a constant real number.</span><span style="font-family: Ubuntu, sans-serif; font-weight: bold;">&nbsp;</span><strong>It is guaranteed that A<sub>0</sub>&nbsp;is an integer.</strong></p>
<p style="font-family: 'Ubuntu', sans-serif; font-size: 14px;"><span style="vertical-align: sub;"><span style="font-family: Ubuntu, sans-serif;">After recieving the doctor's prescription, Watame went home only to realise the reciept has a different array from the recommendation given from the doctor.&nbsp;</span></span></p>
<p style="font-family: 'Ubuntu', sans-serif; font-size: 14px;">What was printed on the reciept was an array of integers <strong>S<sub>i</sub>&nbsp;</strong>with a note that <strong>S<sub>i</sub>&nbsp;= [A<sub>i</sub>].</strong></p>
<p style="font-family: 'Ubuntu', sans-serif; font-size: 14px;">Here,&nbsp;<strong>[x] </strong>denotes the largest integer less than or equal to <strong>x</strong>&nbsp;(floor function).</p>
<p style="font-family: 'Ubuntu', sans-serif; font-size: 14px;">For rehabilitation, Watame is forced to minimize&nbsp;<strong>d</strong>&nbsp;(since minimizing&nbsp;<strong>d</strong>&nbsp;minimizes&nbsp;<strong>A<sub>i</sub>&nbsp;</strong>too, thus less asacoco for Watame) such that the information printed on the reciept is still valid.</p>
<p style="font-family: 'Ubuntu', sans-serif; font-size: 14px;"><strong>If there exists a valid <strong>d</strong>, it</strong>&nbsp;can be represented as a fraction <strong>P / Q </strong>where <strong>GCD(P, Q) = 1</strong>. Print the answer in the form of&nbsp;<strong>P * Q<sup>-1</sup>&nbsp;</strong>modulo <strong>10<sup>9&nbsp;</sup>+ 7</strong>.</p>
<p style="font-family: 'Ubuntu', sans-serif; font-size: 14px;">There can be cases where the reciept can be faulty (the cashier and the doctor may as well be drunk of asacoco) and there is no valid <strong>d</strong>. In this case, print <strong>-1</strong> instead.</p>
<p style="font-size: 18px; font-family: 'Ubuntu', sans-serif; "><strong>Input Format</strong></p>
<p style="font-family: 'Ubuntu', sans-serif; font-size: 14px;">The first line contains an integer&nbsp;<strong>N</strong><strong>, </strong><strong>the size of the array</strong><strong> <strong>S</strong></strong>.</p>
<p style="font-family: 'Ubuntu', sans-serif; font-size: 14px;">The next lines contains <strong>N</strong>&nbsp;integers <strong>S</strong><span style="font-family: Ubuntu, sans-serif; font-size: 14px; font-weight: 700;"><sub>i</sub><sub>.</sub></span></p>
<p style="font-size: 18px; font-family: 'Ubuntu', sans-serif; "><strong>Output Format</strong></p>
<p style="font-size: 14px; font-family: 'Ubuntu', sans-serif; ">Print an integer representing the answer in the form of <strong>P * Q<sup>-1</sup></strong><span style="vertical-align: super;">&nbsp;</span>modulo <strong>10<sup>9</sup>&nbsp;+ 7</strong>.</p>
<p style="font-size: 14px; font-family: 'Ubuntu', sans-serif; ">If there does not exist a valid <strong>d</strong>&nbsp;(the reciept may be faulty), print -1 instead.</p>
<p style="font-size: 18px; font-family: 'Ubuntu', sans-serif; "><strong>Sample Input 1</strong></p>
<p style="font-size: 14px; font-family: 'Ubuntu', sans-serif; ">6</p>
<p style="font-size: 14px; font-family: 'Ubuntu', sans-serif; ">1 2 3 4 5 6</p>
<p style="font-size: 18px; font-family: 'Ubuntu', sans-serif; "><strong>Sample Output 1</strong></p>
<p style="font-size: 14px; font-family: 'Ubuntu', sans-serif; ">1</p>
<p style="font-size: 18px; font-family: Ubuntu, sans-serif;"><strong>Sample Input 2</strong></p>
<p style="font-size: 14px; font-family: Ubuntu, sans-serif;">5</p>
<p style="font-size: 14px; font-family: Ubuntu, sans-serif;">3 3 3 3 4</p>
<p style="font-size: 18px; font-family: Ubuntu, sans-serif;"><strong>Sample Output 2</strong></p>
<p style="font-size: 14px; font-family: Ubuntu, sans-serif;">250000002</p>
<p style="font-size: 18px; font-family: Ubuntu, sans-serif;"><strong>Sample Input 3</strong></p>
<p style="font-size: 14px; font-family: Ubuntu, sans-serif;">2</p>
<p style="font-size: 14px; font-family: Ubuntu, sans-serif;">4 1</p>
<p style="font-size: 18px; font-family: Ubuntu, sans-serif;"><strong>Sample Output 3</strong></p>
<p style="font-size: 14px; font-family: Ubuntu, sans-serif;">-1</p>
<p style="font-size: 14px; font-family: Ubuntu, sans-serif;"><span style="font-family: Ubuntu, sans-serif; font-size: 18px; font-weight: 700;">Explanation</span></p>
<p style="font-size: 14px; font-family: Ubuntu, sans-serif;">The answers for sample 1 and 2 in decimal format is 1.0 and 0.25 respectively.</p>
<p style="font-size: 18px; font-family: 'Ubuntu', sans-serif; "><strong>Constraints</strong></p>
<p style="font-size: 14px; font-family: 'Ubuntu', sans-serif; "><strong>1 ¡Ü&nbsp;N ¡Ü&nbsp;10<sup>5</sup></strong></p>
<p style="font-size: 14px; font-family: 'Ubuntu', sans-serif; "><strong>1&nbsp;<span style="font-family: Ubuntu, sans-serif; font-size: 14px; font-weight: 700;">¡Ü S<sub>i</sub>&nbsp;<span style="font-family: Ubuntu, sans-serif; font-size: 14px; font-weight: 700;">¡Ü 10<sup>9</sup></span></span></strong></p>