## Description

<div><p>Dmitry wrote down $t$ integers on the board, and that is good. He is sure that he lost an <span class="tex-font-style-it">important</span> integer $n$ among them, and that is bad.</p><p>The integer $n$ had the form $\text{10^x}$ ($x \ge 2$), where the symbol '$\text{^}$' denotes exponentiation.. Something went wrong, and Dmitry missed the symbol '$\text{^}$' when writing the <span class="tex-font-style-it">important</span> integer. For example, instead of the integer $10^5$, he would have written $105$, and instead of $10^{19}$, he would have written $1019$.</p><p>Dmitry wants to understand which of the integers on the board could have been the <span class="tex-font-style-it">important</span> integer and which could not.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of integers on the board.</p><p>The next $t$ lines each contain an integer $a$ ($1 \le a \le 10000$)&nbsp;！ the next integer from the board.</p></div><div class="output-specification"><p>For each integer on the board, output "<span class="tex-font-style-tt">YES</span>" if it could have been the <span class="tex-font-style-it">important</span> integer and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You may output each letter in any case (lowercase or uppercase). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be accepted as a positive answer.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of integers on the board.</p><p>The next $t$ lines each contain an integer $a$ ($1 \le a \le 10000$)&nbsp;！ the next integer from the board.</p>

## Output

<p>For each integer on the board, output "<span class="tex-font-style-tt">YES</span>" if it could have been the <span class="tex-font-style-it">important</span> integer and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You may output each letter in any case (lowercase or uppercase). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be accepted as a positive answer.</p>





```input1|2,4,6,8
7
100
1010
101
105
2033
1019
1002
```




```output1
NO
YES
NO
YES
NO
YES
NO
```


