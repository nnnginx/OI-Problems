## Description

<div><p>We call a phone number a <span class="tex-font-style-it">beautiful</span> if it is a string of $10$ digits, where the $i$-th digit from the left is at least $10 - i$. That is, the first digit must be at least $9$, the second at least $8$, $\ldots$, with the last digit being at least $0$.</p><p>For example, <span class="tex-font-style-tt">9988776655</span> is a beautiful phone number, while <span class="tex-font-style-tt">9099999999</span> is not, since the second digit, which is $0$, is less than $8$.</p><p>Vadim has a <span class="tex-font-style-bf">beautiful</span> phone number. He wants to rearrange its digits in such a way that the result is the <span class="tex-font-style-bf">smallest possible beautiful</span> phone number. Help Vadim solve this problem.</p><p>Please note that the phone numbers are compared as integers.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The only line of each test case contains a single string $s$ of length $10$, consisting of digits. It is guaranteed that $s$ is a <span class="tex-font-style-bf">beautiful</span> phone number.</p></div><div class="output-specification"><p>For each test case, output a single string of length $10$ ¡ª the smallest possible beautiful phone number that Vadim can obtain.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The only line of each test case contains a single string $s$ of length $10$, consisting of digits. It is guaranteed that $s$ is a <span class="tex-font-style-bf">beautiful</span> phone number.</p>

## Output

<p>For each test case, output a single string of length $10$ ¡ª the smallest possible beautiful phone number that Vadim can obtain.</p>





```input1|2,4
4
9999999999
9988776655
9988776650
9899999999
```




```output1
9999999999
9876556789
9876567890
9899999999
```



## Note

<p>In the first test case, for the first phone number <span class="tex-font-style-tt">9999999999</span>, regardless of the rearrangement of digits, the same phone number is obtained.</p><p>In the second test case, for the phone number <span class="tex-font-style-tt">9988776655</span>, it can be proven that <span class="tex-font-style-tt">9876556789</span> is the smallest phone number that can be obtained by rearranging the digits.</p>
